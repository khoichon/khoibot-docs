# khoibot's Games

Games are *very* important. Trust me.

## Decrypt

The bot will choose a word, and hide most of the letters. The job of the players is to guess the original word. Every 30 seconds, the bot will reveal another letter. Stuck? `!decrypt hint` gives you a hint, up to 2 per game.

## Anagram

The bot will choose a word, and shuffle the letters, where the players will have to guess the original word. `!anagram hint` gives a hint and `!anagram skip` skips the word.

## Numguess

The bot will choose a number from 1 to the set maximum number, and you will have to guess that number.

Every time you guess a number, the bot will tell you whether its number is higher, lower or is correct.

Use `!numguess [max]` to pick the maximum number, and `!numguess hint` if you need a hint.

## Wordle

One shared 5 letter wordle for the whole group, with 6 guesses. Send a guess with `!wordle <word>`, ask for a hint with `!wordle hint` and give up with `!wordle cancel`.

## Wordchain

Take turns saying a word that starts with the last letter of the one before. `!wordchain cancel` ends the game.

## Math

A math game. The bot asks a question and the first person to send the right answer wins. Start it with `!math [level]`, and leave the level out to get a random one. `!math cancel` ends the game.

The levels are `easy`, `medium`, `hard`, `impossible` and `asian`. A random level never picks impossible or asian, you have to ask for those.

A game ends by itself if nobody gets it in time, and the harder the level the more time you get:

- `easy`: 60 seconds
- `medium`: 90 seconds
- `hard`: 2 minutes
- `impossible`: 3 minutes
- `asian`: 5 minutes

There is also a short cooldown between games in the same group, 20 seconds by default (the bot owner/hoster can change it in `.env`).

## Hot Potato

Pass the potato on before the fuse runs out. Whoever is holding it when it blows up loses. Start a game with `!hotpotato`, and the person holding the potato passes it with `!pass @user`. `!hotpotato cancel` ends it.

## Tournaments

A tournament runs a series of [decrypt](#decrypt) or [math](#math) rounds for the whole group.

- `!tournament create [points]` opens the tournament lobby
- `!tournament join` makes you join the tournament
- `!tournament start [decrypt|math]` starts the rounds
- `!tournament status` shows the current status
- `!tournament cancel` cancels it, as the name implies (its not that hard to understand if you have common sense ;D)

If nobody gets a round in time, the next one starts anyway.

## Tic-tac-toe

Start a match with `!ttt`. The other player can join with `!ttt join`, or you can play the bot with `!ttt ai`. Send a square from 1 to 9 to play your move, and use `!ttt cancel` to stop.

## Rock paper scissors

Play the bot with `!rps <rock|paper|scissors>`.

## Chess

Play another person or the bot. Start with `!chess`, and the other player joins with `!chess join`. To play the bot use `!chess ai [easy|medium|hard]`. Moves are plain messages like `e4` or `Nf3`. `!chess resign` makes you resign, `!chess draw` initiates a draw, and `!chess cancel` stops the game.

## Blackjack and Slots

Casino games are off by default. A mod turns them on with [casinoenabled](moderation#casinoenabled), and they stay separate from the normal games setting.

`!blackjack` deals you a round against the bot. Reply `hit` or `stand`, and use `!blackjack cancel` to stop. `!slots` is a normal slots game.