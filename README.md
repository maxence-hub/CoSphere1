</head>
<body>
    <div class="container">
        <h1 id="welcome-message">Bienvenue</h1>
        <p id="description">
            Connectez-vous pour accéder à votre espace personnel ou créez un compte si vous êtes nouveau.
        </p>
        <button id="login-btn" class="btn btn-primary">Se connecter</button>
        <button id="signup-btn" class="btn btn-secondary">Créer un compte</button>
		<a href="page d'accueil.html" class="btn">Se connecter</a>
    </div>

    <script>
        // Vérifier si un utilisateur est déjà enregistré
        const userRegistered = localStorage.getItem('userRegistered');
        const welcomeMessage = document.getElementById('welcome-message');
        const description = document.getElementById('description');
        const loginBtn = document.getElementById('login-btn');
        const signupBtn = document.getElementById('signup-btn');

        if (userRegistered) {
            // Si un utilisateur est déjà enregistré
            welcomeMessage.textContent = 'Bienvenue de retour !';
            description.textContent = 'Nous sommes heureux de vous revoir. Connectez-vous pour accéder à votre espace.';
            signupBtn.style.display = 'none'; // Cacher le bouton "Créer un compte"
        }

        // Ajouter un événement au bouton "Créer un compte"
        signupBtn.addEventListener('click', () => {
            // Simuler la création d'un compte
            const userName = prompt('Entrez votre nom pour créer un compte :');
            if (userName) {
                localStorage.setItem('userRegistered', userName);
                alert(`Bienvenue, ${userName} ! Votre compte a été créé.`);
                location.reload(); // Recharger la page pour mettre à jour l'interface
            }
        });

        // Ajouter un événement au bouton "Se connecter"
        loginBtn.addEventListener('click', () => {
            if (userRegistered) {
                alert(`Connexion réussie ! Bienvenue, ${userRegistered}.`);
                // Rediriger l'utilisateur vers son espace personnel
                window.location.href = 'dashboard.html';
            } else {
                alert('Veuillez créer un compte avant de vous connecter.');
            }
        });
    </script>
</body>
</html>
