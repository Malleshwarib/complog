<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CompLog - Explore Competitions</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background-color: #fff;
            min-height: 100vh;
        }

        .header-container {
            background: linear-gradient(to right, #8e44ad, #b16bd4);
            color: white;
            padding: 15px 30px;
            border-bottom-left-radius: 40px;
            border-bottom-right-radius: 40px;
        }

        .top-bar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo-icon {
            width: 40px;
            height: 40px;
            background-color: white;
            border-radius: 5px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
        }

        .logo-text {
            font-size: 24px;
            font-weight: bold;
        }

        .admin-section {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .admin-icon {
            width: 35px;
            height: 35px;
            background-color: white;
            border-radius: 5px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .nav {
            display: flex;
            gap: 30px;
            flex-wrap: wrap;
            justify-content: center;
            margin-top: 10px;
        }

        .nav a {
            color: white;
            text-decoration: none;
            font-size: 18px;
        }

        .content-wrapper {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            padding: 20px;
            align-items: stretch;
        }

        .filters {
            background-color: #e0e0e0;
            padding: 20px;
            border-radius: 10px;
            width: 100%;
            max-width: 250px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            flex: 1;
        }

        .filters h2 {
            font-size: 24px;
            margin-bottom: 20px;
        }

        .main-content {
            flex: 3;
            background-color: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            min-width: 300px;
        }

        .content-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 20px;
        }

        .content-title {
            font-size: 28px;
            color: #333;
        }

        .add-button {
            background-color: #4CAF50;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 20px;
            cursor: pointer;
            font-size: 16px;
        }

        .competition-card {
            background-color: #b2dfdb;
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 10px;
        }

        .card-info h3 {
            font-size: 20px;
        }

        .view-button {
            background-color: #90EE90;
            border: none;
            padding: 10px 20px;
            border-radius: 20px;
            cursor: pointer;
        }

        @media (max-width: 768px) {
            .header-container {
                border-radius: 0;
                text-align: center;
            }

            .content-header {
                text-align: center;
                flex-direction: column;
            }

            .competition-card {
                flex-direction: column;
                align-items: center;
                text-align: center;
            }

            .view-button {
                width: 100%;
            }
        }
    </style>
</head>
<body>
    <div class="header-container">
        <div class="top-bar">
            <div class="logo">
                <div class="logo-icon">🏆</div>
                <div class="logo-text">CompLog</div>
            </div>
            <div class="admin-section">
                <span>Admin</span>
                <div class="admin-icon">👤</div>
            </div>
        </div>
        <nav class="nav">
            <a href="#">Home</a>
            <a href="#">Competitions</a>
            <a href="#">Students</a>
            <a href="#">Achievements</a>
            <a href="#">Login</a>
        </nav>
    </div>

    <div class="content-wrapper">
        <aside class="filters">
            <h2>Filters</h2>
            <div class="year-section">
                <h3>- Year</h3>
                <div>
                    <input type="checkbox" id="year2024"> <label for="year2024">2024</label>
                    <input type="checkbox" id="year2025"> <label for="year2025">2025</label>
                </div>
            </div>
        </aside>

        <main class="main-content">
            <div class="content-header">
                <h1 class="content-title">Explore Competitions in Science</h1>
                <button class="add-button">Add</button>
            </div>

            <div class="competition-card">
                <div class="card-info">
                    <h3>Intercollege Science Quiz</h3>
                    <p>ABC college name</p>
                    <p>Date: January 1st,2024</p>
                </div>
                <button class="view-button">View</button>
                <div class="competition-card">
                <div class="card-info">
                    <h3>Intercollege Science Quiz</h3>
                    <p>ABC college name</p>
                    <p>Date: January 1st,2024</p>
                </div>
                <button class="view-button">View</button>
            </div>
        </main>
    </div>
</body>
</html>
