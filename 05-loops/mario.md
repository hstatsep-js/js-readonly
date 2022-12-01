## Itsa me, Mario!

Toward the beginning of World 1-1 in Nintendo’s Super Mario Brothers, Mario must hop over two "half-pyramids" of blocks as he heads toward a flag pole. Below is a screenshot.

![mario](http://www.infendo.com/wp-content/uploads/2008/06/mario.png)

Your mission is to recreate these blocks using code. When you finish a part, feel free to comment certain parts out and move on to the next part.

### Part I: The Boring Pyramid
We want to write a function that will print the following pyramid:

```
   #  #
  ##  ##
 ###  ###
####  ####
```

(The height and the width of the half-pyramids pictured above are 4 with a gap of size 2 separating them.) 

The function `boringPyramid()` is already written; feel free to uncomment it to see it in action.

But there's a cool trick in Javascript that might allow us to do this more efficiently. It's called `.repeat()`

```js
console.log("You are " + "so ".repeat(5) + "awesome!");
// You are so so so so so awesome!
```

Now write refactored code in `boringPyramidRefactored()` using `.repeat()`. Do NOT write a `for` loop. The result should be EXACTLY the same, but you should be using `.repeat()` for spaces and pound symbols.

### Part II: User Specified Height

Add a new feature to your program that asks a user how tall they would like to make the pyramid. This should be a non-negative integer no greater than 23 (this is the tallest that a pyramid can be in Mario land).

### Part III: Chained pyramids

Modify your code to prompt the user for the number of pyramids they want. Using this number, stack the pyramids on top of each other in a chain. This would be an example of a pyramid with height of 4 and chain length of 3:
```
   #  #
  ##  ##
 ###  ###
####  ####
   #  #
  ##  ##
 ###  ###
####  ####
   #  #
  ##  ##
 ###  ###
####  ####
```

### Part IV: Every-Other-Upside-Down Pyramid
Similar to Part III, but make every other pyramid inverted. Example:
```
   #  #
  ##  ##
 ###  ###
####  ####
####  ####
 ###  ###
  ##  ##
   #  #
   #  #
  ##  ##
 ###  ###
####  ####
```

HINT: you can write another helper function if you need to!