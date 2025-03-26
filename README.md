<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>App Store</title>
    <style>
        /* General Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Body styling */
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            color: #333;
            padding: 0;
            margin: 0;
        }

        /* Header Section */
        header {
            background-color: #1E88E5;
            padding: 10px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            color: white;
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
        }

        header .search-bar input {
            padding: 8px;
            border-radius: 20px;
            border: none;
            width: 300px;
        }

        /* Main Section */
        main {
            padding: 20px;
        }

        /* Categories Section */
        .category {
            margin-bottom: 30px;
        }

        .category h2 {
            font-size: 24px;
            margin-bottom: 10px;
        }

        .category-list {
            display: flex;
            gap: 15px;
            overflow-x: auto;
            padding-bottom: 10px;
        }

        .category-item {
            background-color: #ffffff;
            padding: 10px 20px;
            border-radius: 25px;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .category-item:hover {
            background-color: #ccc;
        }

        /* Apps List Section */
        .app-list {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }

        .app-card {
            background-color: #ffffff;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            display: flex;
            flex-direction: column;
        }

        .app-card img {
            width: 100%;
            height: 150px;
            object-fit: cover;
            border-bottom: 1px solid #ddd;
        }

        .app-info {
            padding: 15px;
        }

        .app-info h3 {
            font-size: 18px;
            margin-bottom: 8px;
        }

        .app-info p {
            font-size: 14px;
            color: #666;
            margin-bottom: 10px;
        }

        .app-info .btn {
            padding: 8px;
            background-color: #1E88E5;
            color: white;
            border-radius: 5px;
            text-align: center;
            cursor: pointer;
            text-decoration: none;
        }

        .app-info .btn:hover {
            background-color: #1565C0;
        }

        /* Footer Section */
        footer {
            text-align: center;
            padding: 10px;
            background-color: #1E88E5;
            color: white;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
                /* Global Reset */
                * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Body Styling */
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            color: #333;
        }

        /* Header Styling */
        header {
            background-color: #0d47a1;
            padding: 10px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            color: white;
        }

        header .logo {
            font-size: 24px;
            font-weight: bold;
        }

        header .search-bar input {
            padding: 8px;
            border-radius: 20px;
            border: none;
            width: 250px;
        }

        /* Main Content Area */
        main {
            padding: 20px;
        }

        /* Categories Section */
        .categories {
            margin-bottom: 30px;
        }

        .categories h2 {
            font-size: 24px;
            margin-bottom: 15px;
        }

        .categories .category-list {
            display: flex;
            gap: 15px;
            overflow-x: auto;
        }

        .categories .category-item {
            background-color: #fff;
            padding: 10px 20px;
            border-radius: 30px;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .categories .category-item:hover {
            background-color: #2196f3;
            color: white;
        }

        /* App Cards Section */
        .apps {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }

        .apps .app-card {
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            display: flex;
            flex-direction: column;
        }

        .apps .app-card img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }

        .apps .app-card .app-info {
            padding: 15px;
        }

        .apps .app-card .app-info h3 {
            font-size: 18px;
            margin-bottom: 8px;
        }

        .apps .app-card .app-info p {
            font-size: 14px;
            color: #666;
        }

        .apps .app-card .app-info .install-btn {
            background-color: #0d47a1;
            color: white;
            padding: 10px;
            border-radius: 5px;
            text-align: center;
            cursor: pointer;
            margin-top: 10px;
            text-decoration: none;
            font-weight: bold;
        }

        .apps .app-card .app-info .install-btn:hover {
            background-color: #1565c0;
        }

        /* Footer Styling */
        footer {
            text-align: center;
            padding: 10px;
            background-color: #0d47a1;
            color: white;
        }

    </style>
</head>
<body>

    <!-- Header Section -->
    <header>
        <div class="logo">Playstore</div>
        <div class="search-bar">
            <input type="text" placeholder="Search for apps">
        </div>
    </header>

    <!-- Main Content Section -->
    <main>
        <!-- Categories Section -->
        <section class="category">
            <h2>Categories</h2>
            <div class="category-list">
                <div class="category-item">Games</div>
                <div class="category-item">Music</div>
                <div class="category-item">Social</div>
                <div class="category-item">Productivity</div>
            </div>
        </section>

        <!-- Apps Section -->
        <section class="app-list">
            <h2>Top Apps</h2>

            <!-- App Card 1 -->
            <div class="app-card">
                <img src="https://i.pinimg.com/236x/8e/f9/4b/8ef94b36360769dcf3ab9699bc961445.jpg" alt="App Icon">
                <div class="app-info">
                    <h3>FreeFire</h3>
                    <p>Free Fire is a world-famous survival shooter game available on mobile. Each 10-minute game places you on a remote island where you are pit against 49 other players, all seeking survival. Players freely choose their starting point with their parachute, and aim to stay in the safe zone for as long as possible.!</p><br>
                    <a href="#" class="btn">Install</a>
                </div>
            </div>

            <!-- App Card 2 -->
            <div class="app-card">
                <img src="https://static.vecteezy.com/system/resources/previews/024/474/342/non_2x/travel-bus-logo-template-with-white-background-suitable-for-your-design-need-logo-illustration-animation-etc-free-vector.jpg" alt="App Icon">
                <div class="app-info">
                    <h3>Bus Game</h3>
                    <p>Bus games are typically simulation or driving games where players take on the role of a bus driver, navigating routes, picking up passengers, and managing their bus company. !</p><br><br>
                    <a href="#" class="btn">Install</a><br>
                </div>
            </div>

            <!-- App Card 3 -->
            <div class="app-card">
                <img src="https://t4.ftcdn.net/jpg/05/20/94/61/360_F_520946103_KYIhfgNXGTQLMOkCxRpjMm6epv6IT5Ui.jpg" alt="App Icon">
                <div class="app-info">
                    <h3>Truck Game </h3>
                    <p>Truck games are video games where players take on the role of a truck driver, often tasked with delivering cargo or participating in races, offering a realistic simulation of driving and managing a trucking business. !</p><br>
                    <a href="#" class="btn">Install</a>
                </div>
            </div>

            <!--App Card 4-->
           <div class="app-card">
                <img src="https://cdn.altlabvr.com/23452.jpeggn4t1712601488.jpeg?quality=80&type=jpg&width=1920" alt="App Icon">
                <div class="app-info">
                    <h3>Car Racer game</h3>
                    <p>Car games encompass a variety of activities played during car rides, often to pass the time, and can range from simple spot-the-object games to more complex word or guessing games. </p><br>
                    <a href="#" class="btn">Install</a>
            </div>


            


        </section>
    </main>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2025 Playstore /. Himal</p>
    </footer>
    

</body>
</html>

