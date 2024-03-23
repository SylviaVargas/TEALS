### Tutorial: Understanding Event Handlers in MakeCode Arcade Blocks

In programming, an event handler is a piece of code that is designed to respond to a specific event or action. In Microsoft's MakeCode Arcade Blocks, event handlers are used to respond to user input or other events that occur during the execution of a program. Here's how event handlers work in MakeCode Arcade Blocks, along with some examples:

#### What is an Event Handler?
An event handler is a block of code that is triggered by a specific event. In MakeCode Arcade Blocks, events can include button presses, collisions between sprites, or timers reaching a certain value. When an event occurs, the corresponding event handler is executed, allowing you to define how your program should respond to that event.

#### Example 1: Button Press Event Handler
```blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    // Code to run when button A is pressed
})
```
In this example, the event handler is triggered when button A is pressed on the controller. The `function () { ... }` block contains the code that will be executed when the event occurs.

#### Example 2: Sprite Collision Event Handler
```blocks
sprites.onOverlap(SpriteKind.Player, SpriteKind.Food, function(sprite: Sprite, otherSprite: Sprite) {
    // Code to run when the player sprite overlaps with a food sprite
})
```
In this example, the event handler is triggered when the player sprite overlaps with a food sprite. The `function(sprite: Sprite, otherSprite: Sprite) { ... }` block contains the code that will be executed when the event occurs. The `sprite` and `otherSprite` parameters represent the sprites involved in the collision.

#### Example 3: Timer Event Handler
```blocks
game.onUpdateInterval(2000, function() {
    // Code to run every 2 seconds
})
```
In this example, the event handler is triggered every 2 seconds. The `function() { ... }` block contains the code that will be executed each time the event occurs.

#### Example 4: Shake Event Handler
```blocks
input.onGesture(Gesture.Shake, function () {
    // Code to run when the device is shaken
})
```
In this example, the event handler is triggered when the device is shaken. The `function () { ... }` block contains the code that will be executed when the event occurs.

#### Example 5: Screen Touch Event Handler
```blocks
controller.player1.onButtonEvent(ControllerButton.Up, ControllerButtonEvent.Pressed, function () {
    // Code to run when the up button is pressed
})
```
In this example, the event handler is triggered when the up button is pressed on the player 1 controller. The `function () { ... }` block contains the code that will be executed when the event occurs.

### References

- https://makecode.microbit.org/reference/input/on-button-pressed#:~:text=Start%20an%20event%20handler%20(part,pushing%20down%20the%20second%20button


### Assignment Options
- https://arcade.makecode.com/courses/csintro3/events/buttons-problems
- https://arcade.makecode.com/courses/csintro3/events/buttons


### Quiz

1. What is an event handler?
   - A. A block of code that responds to specific events
   - B. A block of code that runs continuously
   - C. A block of code that defines variables
   - D. A block of code that creates sprites

**Answer:** A. A block of code that responds to specific events

2. Which of the following events can trigger an event handler in MakeCode Arcade Blocks?
   - A. Button presses
   - B. Sprite collisions
   - C. Timer reaching a certain value
   - D. All of the above

**Answer:** D. All of the above

3. What does the following code do?
   ```blocks
   controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
       // Code to run when button A is pressed
   })
   ```
   - A. Responds to a button A press event
   - B. Creates a new sprite
   - C. Starts a timer
   - D. None of the above

**Answer:** A. Responds to a button A press event

4. When does a sprite collision event handler execute?
   - A. When two sprites overlap
   - B. When a sprite is created
   - C. When a timer reaches a certain value
   - D. When a button is pressed

**Answer:** A. When two sprites overlap

5. How often does a timer event handler execute?
   - A. Every second
   - B. Every 2 seconds
   - C. Every time a button is pressed
   - D. Every time a sprite is created

**Answer:** B. Every 2 seconds