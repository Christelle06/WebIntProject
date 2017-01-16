	var fs = require('fs');
	var file = fs.readFileSync('json/recipe.json','utf8');
	var src = JSON.parse(file);
	var data =  JSON.parse('{"name": "Bacon Burger", "recipeIngredient":["1 chopped steak","2 bacon slices","2 cheddar slices","salad","ketchup","mustard"], "recipeInstructions": "Clean the salad, brown the steak. Add the bacon slices in the pan. Heat the bun in the oven for 5 minutes at 180°C. Create your burger with salad, sauces, steak, bacon, and cheddar. Heat it in the oven for 5 minutes at 180°C to melt the cheese."}');
	
	document.getElementById("name").innerHTML = data.name;
	console.log(src);