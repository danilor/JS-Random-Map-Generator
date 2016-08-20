# JS-Random-Map-Generator
Small script to simulate the logic behind the generation of a map.

@Author: Danilo Ramírez Mattey
@Year: 2016
@Disclaimer: Use this script and logic under your own risk. This is a Javascript code, and that means that it can freeze your browser under certain conditions.
	
Please, if you use this code, or part of it, remember to attribute the credit to its author (I mean, me!)
This is just an example and with edutational purposes. I will update the logic as soon as I get a better way to solve some issues.
I am not native english speaker, so this code may have spelling errors.

## Use
The idea is just to load the index.html file in a browser that can run javascript (the faster, the better) [I recommend Chrome for this kind of testing].

While working, it will display all the process in the console. That means that if you open the console of the browser while loading, you will see every single step that the application is taking in order to generate the map. But having the console open means that the page will load a lot slower since it has to send all console messages to the browser.

## Configuration

There are 2 areas that requiere configuration: the main area (where the map is actually defined) and the blocks area (where it is defined the types of terrain accepted). All this information can be found in the javascript section of the page. (again, this code requires a little knowledge of programming).

### Main Area

Here you can configure the following:

+ total_x = This is the width of the map (larger number, larger amount of time to process)
+ total_y = This is the height of the map (larger number, larger amount of time to process)
+ tolerance = This is the number of revisions the code will make after the creation of the map.

### Blocks area

The definition of the terrain types that the map can have, can be found in the function: setBasicElements(). This function set up the information of each basic terrain type in the following format:

      //Forest
			var v = new Object();
			v.class = 'forest_space';
			v.letter = 'f';
			v.max = 30;
			v.added = [];
			basic_elements.push(v);
			
Each type of terrain must have its equivalent in the CSS (styling) area.

## Contact

You can ask me questions here in Github (if any).

## Requirements

+ Jquery 2.2.4 (its embeded in the code as an external reference). 
