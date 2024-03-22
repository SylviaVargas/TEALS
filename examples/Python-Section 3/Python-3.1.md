# Global variables
hero_sprite: Sprite = None

def create_hero_sprite():
    global hero_sprite
    hero_sprite = sprites.create(assets.image("""hero"""), SpriteKind.player)
    hero_sprite.set_position(80, 100)
    hero_sprite.set_flag(SpriteFlag.STAY_IN_SCREEN, True)
    controller.move_sprite(hero_sprite)
    info.set_score(0)

# on start
create_hero_sprite()