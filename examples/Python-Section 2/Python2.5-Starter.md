## Create a sprite from an image saved to MyAssets
mySprite = sprites.create(assets.image("""
    myImage
"""), SpriteKind.player)

## Ask for the name of the player 
sprite_name = game.ask_for_string("What is your name?")

## The sprite says Hello to the player with their name.
message = "Hello " + sprite_name 
mySprite.say_text(message )
