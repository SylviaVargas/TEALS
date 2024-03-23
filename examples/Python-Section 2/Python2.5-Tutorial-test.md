# Python 2.5 - Overview 

### @explicitHints true

## Introduction @unplugged

We will be reviewing **animation** by
- Part 1: Creating assets
- Part 2: Attaching the assets to a sprite
- Part 3: Stopping the animation

## Step 0 

Create a sprite with any image.  Use the default from the Toolbox!

```python
# @validate-exists 
 mySprite = sprites.create(assets.image("""
    smallApple
    """), SpriteKind.player)
```

## Step: Create an animation
```python
animation.run_image_animation(None, [], 500, False)
```



## Step 1

Put in an ``||input:on button pressed||`` event to run code when the controller button **A** is pressed.

```python
def on_a_pressed():
    pass
controller.A.on_event(ControllerButtonEvent.PRESSED, on_a_pressed)
```

## Step 2

Use ``||run_image_animation|`` to display the animation on the screen.

Press the **A** button in the simulator to see the animation you created.

```python
def on_a_pressed():
    animation.run_image_animation(hero_sprite,
        assets.animation("""my_animation"""), 500, True)
controller.A.on_event(ControllerButtonEvent.PRESSED, on_a_pressed)

```

## Step 3

Use another ``||input:on button pressed||`` with a ``||basic:show icon||`` inside to display a **Sad** face when button **B** is pressed.

```python
def on_button_pressed_a2():
    basic.show_icon(IconNames.SAD)
input.on_button_pressed(Button.B, on_button_pressed_a2)
```

## Step 4

Add a secret mode that happens when **A** and **B** are pressed together. For this case, use ``||basic:show icon||`` multiple times to create an animation.

```python
def on_button_pressed_a3():
    basic.show_icon(IconNames.SILLY)
    basic.show_icon(IconNames.SURPRISED)
input.on_button_pressed(Button.AB, on_button_pressed_a3)
```

## Finish

