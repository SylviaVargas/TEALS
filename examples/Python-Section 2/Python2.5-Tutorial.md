 # Python Lab 2.5 - Activity 4: For loops

## Step 1: Creating Assets
1. Create an image for your sprite and add it to the Asset Manager.
 - https://arcade.makecode.com/reference/sprites/sprite/set-image 
 - https://arcade.makecode.com/reference/sprites/create


 ```
 ## Create a Sprite.  The example is an Apple.
 
 mySprite = sprites.create(assets.image("""
    smallApple
    """), SpriteKind.player)
 ```
2. Create an animation for your sprite and add it to  the asset. See https://arcade.makecode.com/types/animation 

In the Python editor, write a **for** loop from 1 to 10 which writes to the screen 1 to 10.

In the **for loop** use the function [range](https://www.w3schools.com/python/ref_func_range.asp)

``` python
for counter in range(10):
    game.splash(counter)
``` 
 ## STEP 2
Run the project to see that it works.
Remember to click on the "A" button to advance to the next number.
