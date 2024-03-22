# Bell Ringer
1.	Open a new MakeCode Arcade Project in Python and call it “Bell Ringer 3.2.”
2.	Create a new String variable called greeting and initialize it to give a greeting.
3.	Create a new function called change_greeting(), which takes no parameters and returns nothing. Change greeting in this function to some other string.
4.	Create a new Player sprite, with any picture you choose.
5.	Call your change_greeting() function, then have your sprite say greeting.


- https://youtu.be/wueXfiVkw1I?si=atTb9lWOvv4kPf4K 
Python 3 Tutorial for Beginners # 13 Variable Scope

- Python Tutorial: Variable Scope - Understanding the LEGB
https://www.google.com/search?q=Tutorial+on+Python+variable+scope&oq=Tutorial+on+Python+variable+scope&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIHCAEQIRigATIHCAIQIRigAdIBCTE1MTQ0ajBqMagCALACAA&sourceid=chrome&ie=UTF-8&safe=active&ssui=on#fpstate=ive&vld=cid:40c77429,vid:QVdf0LgmICw,st:0
# Variables
greeting : string = "Hello, world!"

hero_sprite : Sprite = sprites.create(img("""
    . . . . . . . . . . b 5 b . . .
    . . . . . . . . . b 5 b . . . .
    . . . . . . . . . b c . . . . .
    . . . . . . b b b b b b . . . .
    . . . . . b b 5 5 5 5 5 b . . .
    . . . . b b 5 d 1 f 5 5 d f . .
    . . . . b 5 5 1 f f 5 d 4 c . .
    . . . . b 5 5 d f b d d 4 4 . .
    b d d d b b d 5 5 5 4 4 4 4 4 b
    b b d 5 5 5 b 5 5 4 4 4 4 4 b .
    b d c 5 5 5 5 d 5 5 5 5 5 b . .
    c d d c d 5 5 b 5 5 5 5 5 5 b .
    c b d d c c b 5 5 5 5 5 5 5 b .
    . c d d d d d d 5 5 5 5 5 d b .
    . . c b d d d d d 5 5 5 b b . .
    . . . c c c c c c c c b b . . .
"""), SpriteKind.player)

# Functions
def change_greeting():
    greeting = "Hola Mundo!"

change_greeting()
hero_sprite.say_text(greeting)


# Step 1
# Variables
hero_sprite : Sprite = sprites.create(img("""
    . . . . . . . . . . b 5 b . . .
    . . . . . . . . . b 5 b . . . .
    . . . . . . . . . b c . . . . .
    . . . . . . b b b b b b . . . .
    . . . . . b b 5 5 5 5 5 b . . .
    . . . . b b 5 d 1 f 5 5 d f . .
    . . . . b 5 5 1 f f 5 d 4 c . .
    . . . . b 5 5 d f b d d 4 4 . .
    b d d d b b d 5 5 5 4 4 4 4 4 b
    b b d 5 5 5 b 5 5 4 4 4 4 4 b .
    b d c 5 5 5 5 d 5 5 5 5 5 b . .
    c d d c d 5 5 b 5 5 5 5 5 5 b .
    c b d d c c b 5 5 5 5 5 5 5 b .
    . c d d d d d d 5 5 5 5 5 d b .
    . . c b d d d d d 5 5 5 b b . .
    . . . c c c c c c c c b b . . .
"""), SpriteKind.player)

greeting = "Hello, world!"
# Functions


# On Start 
hero_sprite.say_text(greeting)

# Step 2: Create a function to change the greeting

# Variables
hero_sprite : Sprite = sprites.create(img("""
    . . . . . . . . . . b 5 b . . .
    . . . . . . . . . b 5 b . . . .
    . . . . . . . . . b c . . . . .
    . . . . . . b b b b b b . . . .
    . . . . . b b 5 5 5 5 5 b . . .
    . . . . b b 5 d 1 f 5 5 d f . .
    . . . . b 5 5 1 f f 5 d 4 c . .
    . . . . b 5 5 d f b d d 4 4 . .
    b d d d b b d 5 5 5 4 4 4 4 4 b
    b b d 5 5 5 b 5 5 4 4 4 4 4 b .
    b d c 5 5 5 5 d 5 5 5 5 5 b . .
    c d d c d 5 5 b 5 5 5 5 5 5 b .
    c b d d c c b 5 5 5 5 5 5 5 b .
    . c d d d d d d 5 5 5 5 5 d b .
    . . c b d d d d d 5 5 5 b b . .
    . . . c c c c c c c c b b . . .
"""), SpriteKind.player)

greeting = "Hello, world!"
# Functions


# On Start 
hero_sprite.say_text(greeting)


