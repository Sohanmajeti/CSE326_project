<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Recipe Book</title>
    <style>
        /* General styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #108d93;
        }

        header {
            background-color: #39e0ec;
            padding: 20px;
            text-align: center;
            color: white;
        }

        header h1 {
            margin: 0;
        }

        #search-bar {
            padding: 10px;
            width: 80%;
            max-width: 400px;
            margin-top: 10px;
            border: none;
            border-radius: 5px;
            font-size: 16px;
        }

        #ingredient-filter {
            padding: 20px;
            text-align: center;
        }

        #ingredient-filter label {
            margin-right: 20px;
            font-size: 18px;
        }

        #type-of {
            padding: 20px;
            text-align: center;
        }

        #type-of label {
            margin-right: 20px;
            font-size: 18px;
        }

        #recipe-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .recipe-card {
            background-color: rgb(46, 167, 195);
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            text-align: center;
            transition: transform 0.3s;
        }

        .recipe-card:hover {
            transform: translateY(-5px);
        }

        .recipe-card img {
            width: 100%;
            border-radius: 10px;
        }

        .recipe-card h3 {
            margin-top: 15px;
            color: #333;
        }

        .recipe-card p {
            color: #1f0202;
        }
    </style>
</head>
<body>

    <header>
        <h1>My Recipe Book</h1>
        <input type="text" id="search-bar" placeholder="Search for a recipe...">
    </header>

    <section id="ingredient-filter">
        <h2>Filter by Ingredient</h2>
        <label><input type="checkbox" value="eggs"> Eggs</label>
        <label><input type="checkbox" value="flour"> Flour</label>
        <label><input type="checkbox" value="sugar"> Sugar</label>
        <label><input type="checkbox" value="bread"> Bread</label>
        <label><input type="checkbox" value="water"> Water</label>
    </section>

    <section id="recipe-list">
        <article class="recipe-card">
            <img src="pancakes.jpg" alt="Recipe Image">
            <h3>Pancakes</h3>
            <p>Fluffy and delicious pancakes perfect for breakfast.</p>
        </article>
        <article class="recipe-card">
            <img src="omelette.jpg" alt="Recipe Image">
            <h3>Omelette</h3>
            <p>A simple omelette packed with protein.</p>
        </article>
        <article class="recipe-card">
            <img src="brownies.jpg" alt="Recipe Image">
            <h3>Brownies</h3>
            <p>Rich and fudgy chocolate brownies.</p>
        </article>
        <article class="recipe-card">
            <img src="french.jpg" alt="Recipe Image">
            <h3>French toast</h3>
            <p>Simple and sweet breakfast.</p>
        </article>
        <article class="recipe-card">
            <img src="gulab jamun.jpg" alt="Recipe Image">
            <h3>Gulab jamun</h3>
            <p>Sweet and soft dessert.</p>
        </article>

    </section>

</body>
</html>
