<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Accueil - Votre Application</title>
    <style>
        /* Styles de base */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #4a90e2, #9013fe);
            color: #fff;
            display: flex;
            flex-direction: row;
            min-height: 100vh;
        }

        /* Barre latérale */
        .sidebar {
            width: 300px;
            background: rgba(255, 255, 255, 0.1);
            box-shadow: 2px 0 10px rgba(0, 0, 0, 0.2);
            padding: 20px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .sidebar h2 {
            font-size: 1.5rem;
            margin-bottom: 20px;
            text-align: center;
            color: #fff;
        }

        .sidebar ul {
            list-style: none;
            padding: 0;
        }

        .sidebar ul li {
            margin: 10px 0;
        }

        .sidebar ul li a {
            text-decoration: none;
            color: #dcdcdc;
            font-size: 1rem;
            padding: 10px;
            display: block;
            border-radius: 6px;
            transition: all 0.3s ease;
        }

        .sidebar ul li a:hover {
            background: #9013fe;
            color: #fff;
        }

        .sidebar footer {
            font-size: 0.9rem;
            color: #dcdcdc;
            text-align: center;
        }

        /* Contenu principal */
        .main-content {
            flex: 1;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 20px;
        }

        header {
            text-align: center;
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
        }

        header p {
            font-size: 1.2rem;
            color: #dcdcdc;
        }

        .container {
            text-align: center;
            padding: 30px 20px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
            width: 90%;
            max-width: 800px;
        }

        .container h2 {
            font-size: 1.8rem;
            margin-bottom: 20px;
        }

        .btn {
            display: inline-block;
            padding: 12px 20px;
            margin: 10px;
            font-size: 1rem;
            font-weight: bold;
            text-transform: uppercase;
            text-decoration: none;
            border: none;
            border-radius: 6px;
            cursor: pointer;
            background: #4a90e2;
            color: #fff;
            transition: all 0.3s ease, transform 0.1s ease;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        }

        .btn:hover {
            background: #357ABD;
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.3);
            transform: translateY(-3px);
        }

        .btn-secondary {
            background: #9013fe;
        }

        .btn-secondary:hover {
            background: #7311C6;
        }
    </style>
</head>
<body>
    <!-- Barre latérale -->
    <aside class="sidebar">
        <h2>Services</h2>
        <ul>
            <li><a href="history.html">Historique des appels</a></li>
            <li><a href="report.html">Rapport d'activités</a></li>
            <li><a href="chat.html">Discussion en ligne</a></li>
            <li><a href="forum.html">Forum</a></li>
            <li><a href="portal.html">Portail entreprise</a></li>
            <li><a href="feedback.html">Suggestions des utilisateurs</a></li>
        </ul>
        <footer>
            &copy; 2024 Votre Application - Tous droits réservés.
        </footer>
    </aside>

    <!-- Contenu principal -->
    <div class="main-content">
        <header>
            <h1>CoSphere</h1>
            <p>Des réunions simplifiées, où que vous soyez</p>
        </header>

        <div class="container">
            <h2>Bienvenue !</h2>
            <p>Rejoignez une réunion en un clic ou créez la vôtre pour collaborer facilement avec vos collègues et amis.</p>
            <a href="join.html" class="btn">Rejoindre une réunion</a>
            <a href="create.html" class="btn btn-secondary">Organiser une réunion</a>
        </div>
    </div>
</body>
</html>
