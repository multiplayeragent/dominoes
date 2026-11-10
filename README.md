# Dominoes

Match the ends. Empty your hand. First to 100. A multiplayer starter game from [Multiplayer Agent](https://multiplayeragent.com): 2D, turn-based, 2–4 players, with bots that fill empty seats.

![Dominoes](poster.jpg)

## How it plays

Play a tile that matches a number at either end of the line; no match, draw from the boneyard. Empty your hand to win the round and score every pip left in the other hands. First to 100 points wins.

**Controls:** Click or tap a tile to play it (tap an end if it fits both), tap the boneyard to draw.

## Make it yours in the Game Builder

Open the [Game Builder](https://multiplayeragent.com), choose **Start from a starter game** and pick Dominoes. It opens as version 1 in your studio, ready to play and publish. Then ask for changes, for example:

- Score only rounds that end on a multiple of five
- Use a double-nine set for bigger games
- Make the tiles glow like neon on a dark table

## Run it yourself

1. Get a free publishable key (`pk_…`) at [multiplayeragent.com](https://multiplayeragent.com).
2. In `index.html`, put it in place of `pk_REPLACE_ME` in the `MP_CONNECT` block.
3. Open `index.html` in a browser. No build step and no server needed.

Without a key it still runs, offline against bots.

## How it is built

- One `index.html`. The comment at the top of the script maps the code and explains the multiplayer.
- **Hidden info:** Your hand is sealed so only you can read it (the host deals, so it can too).
- **Host-run rules:** The host's browser shuffles, deals and checks every tile; if it leaves, the next player takes over.
- **Bots:** Bots fill empty seats and take over for anyone who leaves.
- **Leaderboard:** Points won, added up over every round, shown after each round.
- `?attract` runs it offline with bots only. The preview video is recorded from it.

## License

MIT.
