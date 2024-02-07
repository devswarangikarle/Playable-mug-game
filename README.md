# Playable-mug-game
Rohan has come up with an intriguing game for his friends. The game starts with a table laid out with an empty cup and n water mugs. Players take their turns sequentially. In each turn, a player selects one of the water mugs and pours all its contents into the cup. 


def can_play_game(n, s, mug_volumes):
    total_mug_volume = sum(mug_volumes)

    if total_mug_volume - max(mug_volumes) <= s:
        print("Yes")
    else:
        print("No")

n, s = map(int, input().split())
mug_volumes = list(map(int, input().split()))

can_play_game(n, s, mug_volumes)
