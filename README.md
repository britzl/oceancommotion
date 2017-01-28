# Ocean Commotion
This project is a test-bed for toying with match-3 game mechanics. It is currently partially modelled after "Candy Crush" with implementation of a few boosters and a bomb. This particular version is a clone of the [original Ocean Commotion Defold example](https://github.com/defold/defold-examples/tree/master/ocean-commotion), adapted for the Defold training in London on the 27th and 28th of January 2017.

The game currently generates special fish for the following matches:

* Match four in a row horizontally to create a striped fish that when triggered removes all fishes in a row
* Match four in a row vertically to create a striped fish that when triggered removes all fish in a column
* Create a T or L shaped match to create a wrapped fish that when triggered removes all adjacent fish
* Match five or more in a row to create a starfish that when triggered removes all fish of a specific color

The game currently implements the special effects for when triggering a match between a striped fish and a normal fish and when combining two wrapped fish (resulting in a horizontal and a vertical lineblast). 

## Suggested exercises
1. Implement one or more of the following special matches:
 1. The effect when matching a wrapped fish with a fish (remove all adjacent fish)
 2. The effect when matching a starfish with a fish (remove all fish of the matched color)
 3. The effect when matching a wrapped fish with a wrapped fish (remove all fish in a radius of 2)
 4. The effect when matching a wrapped fish with a striped fish (remove three rows/columns instead of one)
 5. The effect when matching two starfish (remove all fish)
 6. The effect when a starfish is removed as the result of a lineblast, wrapped explosion or similar (remove all fish of the most common color)
2. Change the board setup so it generates a board with no matches on start.
3. Add scoring for various kinds of matches (3 of a kind, 4 of a kind etc)
4. Prevent illegal moves (that does not lead to a match). Deal with any implications of that new mechanic to make sure that the player never gets stuck.
5. It is currently possible to mess with the data by making a move while the game is dealing with matches. Solve that.

## Improved version
An improved version of the game with some of the above features implemented can be found in the 'improved' branch. The improved version implements:

* 1.1 Wrapped+fish
* 1.2 Starfish+fish
* 1.3 Wrapped+wrapped
* 1.4 Wrapped+striped
* 1.5 Starfish+starfish
* 1.6 Indirect removal of starfish
* 5 Prevent user interaction 
