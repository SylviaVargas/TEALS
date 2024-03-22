### Tutorial: Creating a Horizontal Tile Map in MakeCode Arcade

In MakeCode Arcade, you can create tile maps to design game levels using blocks. Here's a simple tutorial to create a tile map that moves horizontally:

#### Step 1: Create a New Project
1. Go to the MakeCode Arcade website: [arcade.makecode.com](https://arcade.makecode.com/).
2. Click on "New Project" to create a new game project.

#### Step 2: Set Up the Tile Map
1. Click on the "SCENE" tab at the top to enter the scene editor.
2. Click on "SCENE" in the toolbox to add a new scene.
3. Click on the "SCENE" tab again to go back to the scene editor.
4. Click on "TILES" in the toolbox to add a new tile sheet. You can use the default tile sheet or upload your own.
5. Draw your tile map by clicking and dragging tiles onto the scene grid. Create a simple horizontal path for your character to move along.

#### Step 3: Add a Player Character
1. Click on the "SPRITES" tab at the top to enter the sprite editor.
2. Click on "BADDIE" in the toolbox to add a new sprite. This will be your player character.
3. Customize the appearance of your player character using the sprite editor tools.
4. Click on the "CODE" tab to return to the code editor.

#### Step 4: Code the Horizontal Movement
1. Use the "on game update" block from the "MAIN" category to continuously check for input and update the position of the player character.
2. Use an "if" block to check if the player is pressing the left or right arrow keys.
3. Use a "change x by" block to move the player character left or right based on the arrow key pressed.

#### Step 5: Test Your Game
1. Click on the "SCENE" tab to return to the scene editor.
2. Click on the "START" button to test your game. Use the arrow keys to move your player character along the horizontal path.

#### Example Code:
```blocks
controller.moveSprite(BADDIE, 100, 0);

scene.setBackgroundColor(9);

game.onUpdate(function () {
    if (controller.left.isPressed()) {
        BADDIE.x += -2;
    } else if (controller.right.isPressed()) {
        BADDIE.x += 2;
    }
});
```

### Further Exploration:
- Add obstacles to your tile map that the player character must avoid.
- Create a goal for the player character to reach at the end of the horizontal path.
- Experiment with different tile map designs and player character movements to create more complex levels.