# From : https://arcade.makecode.com/types/animation
class SpriteKind(Enum):
    Player = 0
    Enemy = 1
class ActionKind(Enum):
    Walking = 0
    Idle = 1
    Jumping = 2
    Running = 3
runner: animation.Animation = None
walker: animation.Animation = None
mySprite: Sprite = None
walk = False
walk = True
mySprite = sprites.create(img("""
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . . 
        . . . . . . . . . . . . . . . .
    """),
    SpriteKind.Player)
walker = animation.create_animation(ActionKind.Walking, 1000)
walker.add_animation_frame(img("""
    d d d d d d f f f f d d d d d d 
    d d d d f f f 2 2 f f f d d d d 
    d d d f f f 2 2 2 2 f f f d d d 
    d d f f f e e e e e e f f f d d 
    d d f f e 2 2 2 2 2 2 e e f d d 
    d d f e 2 f f f f f f 2 e f d d 
    d d f f f f e e e e f f f f d d 
    d f f e f b f 4 4 f b f e f f d 
    d f e e 4 1 f d d f 1 4 e e f d 
    d d f e e d d d d d d e e f d d 
    d d d f e e 4 4 4 4 e e f d d d 
    d d e 4 f 2 2 2 2 2 2 f 4 e d d 
    d d 4 d f 2 2 2 2 2 2 f d 4 d d 
    d d 4 4 f 4 4 5 5 4 4 f 4 4 d d 
    d d d d d f f f f f f d d d d d 
    d d d d d f f d d f f d d d d d
"""))
walker.add_animation_frame(img("""
    d d d d d d d d d d d d d d d d 
    d d d d d d f f f f d d d d d d 
    d d d d f f f 2 2 f f f d d d d 
    d d d f f f 2 2 2 2 f f f d d d 
    d d f f f e e e e e e f f f d d 
    d d f f e 2 2 2 2 2 2 e e f d d 
    d f f e 2 f f f f f f 2 e f f d 
    d f f f f f e e e e f f f f f d 
    d d f e f b f 4 4 f b f e f d d 
    d d f e 4 1 f d d f 1 4 e f d d 
    d d d f e 4 d d d d 4 e f e d d 
    d d f e f 2 2 2 2 e d d 4 e d d 
    d d e 4 f 2 2 2 2 e d d e d d d 
    d d d d f 4 4 5 5 f e e d d d d 
    d d d d f f f f f f f d d d d d 
    d d d d f f f d d d d d d d d d
"""))
walker.add_animation_frame(img("""
    d d d d d d f f f f d d d d d d 
    d d d d f f f 2 2 f f f d d d d 
    d d d f f f 2 2 2 2 f f f d d d 
    d d f f f e e e e e e f f f d d 
    d d f f e 2 2 2 2 2 2 e e f d d 
    d d f e 2 f f f f f f 2 e f d d 
    d d f f f f e e e e f f f f d d 
    d f f e f b f 4 4 f b f e f f d 
    d f e e 4 1 f d d f 1 4 e e f d 
    d d f e e d d d d d d e e f d d 
    d d d f e e 4 4 4 4 e e f d d d 
    d d e 4 f 2 2 2 2 2 2 f 4 e d d 
    d d 4 d f 2 2 2 2 2 2 f d 4 d d 
    d d 4 4 f 4 4 5 5 4 4 f 4 4 d d 
    d d d d d f f f f f f d d d d d 
    d d d d d f f d d f f d d d d d
"""))
walker.add_animation_frame(img("""
    d d d d d d d d d d d d d d d d 
    d d d d d d f f f f d d d d d d 
    d d d d f f f 2 2 f f f d d d d 
    d d d f f f 2 2 2 2 f f f d d d 
    d d f f f e e e e e e f f f d d 
    d d f e e 2 2 2 2 2 2 e f f d d 
    d f f e 2 f f f f f f 2 e f f d 
    d f f f f f e e e e f f f f f d 
    d d f e f b f 4 4 f b f e f d d 
    d d f e 4 1 f d d f 1 4 e f d d 
    d d e f e 4 d d d d 4 e f d d d 
    d d e 4 d d e 2 2 2 2 f e f d d 
    d d d e d d e 2 2 2 2 f 4 e d d 
    d d d d e e f 5 5 4 4 f d d d d 
    d d d d d f f f f f f f d d d d 
    d d d d d d d d d f f f d d d d
"""))
animation.attach_animation(mySprite, walker)
runner = animation.create_animation(ActionKind.Running, 250)
runner.add_animation_frame(img("""
    d d d d d d f f f f d d d d d d 
    d d d d f f f 2 2 f f f d d d d 
    d d d f f f 2 2 2 2 f f f d d d 
    d d f f f e e e e e e f f f d d 
    d d f f e 2 2 2 2 2 2 e e f d d 
    d d f e 2 f f f f f f 2 e f d d 
    d d f f f f e e e e f f f f d d 
    d f f e f b f 4 4 f b f e f f d 
    d f e e 4 1 f d d f 1 4 e e f d 
    d d f e e d d d d d d e e f d d 
    d d d f e e 4 4 4 4 e e f d d d 
    d d e 4 f 2 2 2 2 2 2 f 4 e d d 
    d d 4 d f 2 2 2 2 2 2 f d 4 d d 
    d d 4 4 f 4 4 5 5 4 4 f 4 4 d d 
    d d d d d f f f f f f d d d d d 
    d d d d d f f d d f f d d d d d
"""))
runner.add_animation_frame(img("""
    d d d d d d d d d d d d d d d d 
    d d d d d d f f f f d d d d d d 
    d d d d f f f 2 2 f f f d d d d 
    d d d f f f 2 2 2 2 f f f d d d 
    d d f f f e e e e e e f f f d d 
    d d f f e 2 2 2 2 2 2 e e f d d 
    d f f e 2 f f f f f f 2 e f f d 
    d f f f f f e e e e f f f f f d 
    d d f e f b f 4 4 f b f e f d d 
    d d f e 4 1 f d d f 1 4 e f d d 
    d d d f e 4 d d d d 4 e f e d d 
    d d f e f 2 2 2 2 e d d 4 e d d 
    d d e 4 f 2 2 2 2 e d d e d d d 
    d d d d f 4 4 5 5 f e e d d d d 
    d d d d f f f f f f f d d d d d 
    d d d d f f f d d d d d d d d d
"""))
runner.add_animation_frame(img("""
    d d d d d d f f f f d d d d d d 
    d d d d f f f 2 2 f f f d d d d 
    d d d f f f 2 2 2 2 f f f d d d 
    d d f f f e e e e e e f f f d d 
    d d f f e 2 2 2 2 2 2 e e f d d 
    d d f e 2 f f f f f f 2 e f d d 
    d d f f f f e e e e f f f f d d 
    d f f e f b f 4 4 f b f e f f d 
    d f e e 4 1 f d d f 1 4 e e f d 
    d d f e e d d d d d d e e f d d 
    d d d f e e 4 4 4 4 e e f d d d 
    d d e 4 f 2 2 2 2 2 2 f 4 e d d 
    d d 4 d f 2 2 2 2 2 2 f d 4 d d 
    d d 4 4 f 4 4 5 5 4 4 f 4 4 d d 
    d d d d d f f f f f f d d d d d 
    d d d d d f f d d f f d d d d d
"""))
runner.add_animation_frame(img("""
    d d d d d d d d d d d d d d d d 
    d d d d d d f f f f d d d d d d 
    d d d d f f f 2 2 f f f d d d d 
    d d d f f f 2 2 2 2 f f f d d d 
    d d f f f e e e e e e f f f d d 
    d d f e e 2 2 2 2 2 2 e f f d d 
    d f f e 2 f f f f f f 2 e f f d 
    d f f f f f e e e e f f f f f d 
    d d f e f b f 4 4 f b f e f d d 
    d d f e 4 1 f d d f 1 4 e f d d 
    d d e f e 4 d d d d 4 e f d d d 
    d d e 4 d d e 2 2 2 2 f e f d d 
    d d d e d d e 2 2 2 2 f 4 e d d 
    d d d d e e f 5 5 4 4 f d d d d 
    d d d d d f f f f f f f d d d d 
    d d d d d d d d d f f f d d d d
"""))
animation.attach_animation(mySprite, runner)

def on_update_interval():
    global walk
    if walk:
        animation.set_action(mySprite, ActionKind.Walking)
    else:
        animation.set_action(mySprite, ActionKind.Running)
    walk = not (walk)
game.on_update_interval(4000, on_update_interval)