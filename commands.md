# khoibot's commands

## Current Commands

- **!ping**

Test if the bot is up. Will also respond with latency in ms.

- **!help**

Shows a help message. Or does it?

- **!decrypt**

Starts a game of [decrypt](gms#decrypt).

- **!anagram**

Starts a game of [anagram](gms#anagram).

- **!coin**

Flips a coin.

- **!roll**

Takes in two types of inputs: \[sides\] or \[count\]d\[sides\]

It will roll that number of dice with that number of sides.

- **!rps**

Takes in 1 input: *rock/paper/scissors*. Can be shortened by putting only the first letter.
Plays rock-paper-scissors with the bot.

- **!ttt**

Starts a tic-tac-toe match. Other player can join with `!ttt join`.

- **!numguess**

Starts a [game where you have to guess the number the bot chose.](gms#numguess)

- **!wordle**

Starts a game of [Wordle](https://www.nytimes.com/2022/02/10/crosswords/best-wordle-tips.html).

- **!ai**

Chats with the AI. It follows the conversation in the group. Use `!ai imagine <description>` to draw a picture, `!ai story <idea>` for a short story and `!ai personality preset <name>` to change how it talks.

- **!summarise**

Summarises some text, a message you reply to, or the last few messages in the group. Give it a number to pick how many messages.

- **!blackjack**

Plays [blackjack](gms#blackjack-and-slots) against the bot. Reply `hit` or `stand`. `!blackjack cancel` ends the round.

- **!slots**

Your normal slots game. Needs casino games turned on, same as blackjack.

- **!chess**

Starts a game of [chess](gms#chess). Other player can join with `!chess join`, or play the bot with `!chess ai`.

- **!wordchain**

Starts a game of [word chain](gms#wordchain).

- **!math**

Starts a [math game](gms#math). Pick a level with `!math easy/medium/hard/impossible/asian`, or leave it out and automatically pickes one for you.

- **!hotpotato**

Starts a game of [hot potato](gms#hot-potato).

- **!pass**

Passes the hot potato to someone with `!pass @user`. If you don't mention anyone it goes back to whoever passed it to you. Only the person holding the potato can pass it.

- **!tournament**

Runs a decrypt or math [tournament](gms#tournaments) for the group.

- **!translate**

Translates some text into the language you pick: `!translate <language> <text>`. You can also reply to a message.

- **!tts**

Draws text on a sticker: `!tts [font] <text>`, or reply to a message. Run it on its own to see the fonts and the animated styles.

- **!edit**

Edits an image or sticker with crop, cut, draw and text. Run it on its own to see the full help.

- **!sticker**

Turns an image into a sticker.

- **!animsticker**

Turns a video or gif into an animated sticker.

- **!calc**

Does maths for you. It knows the usual stuff (+ - * / ^), % and mod for remainders, ! for factorials, brackets, and functions like sqrt, sin, log and round. Also has the constants pi, e and tau.

- **!plot**

Plots a maths expression and sends the graph.

- **!joke**

Sends a random joke.

- **!fact**

Sends a random fact.

- **!quote**

Quotes some text and mentions you. You can also reply to a message.

- **!roast**

A short, friendly roast. About you if you leave it blank, or use `!roast @user`.

- **!compliment**

A short compliment. Works like !roast.

- **!cat**

Sends a random cat photo.

- **!dog**

Sends a random dog photo.

- **!scp**

Looks up an SCP item by number, like `!scp 123`.

- **!define**

Looks up the definition of a word.

- **!wiki**

Sends a Wikipedia summary.

- **!weather**

Shows the weather for a place.

- **!plane**

Shows plane photos and their name/model.

- **!pfp**

Looks up someone's profile picture from their number.

- **!whoami**

Shows your phone number, your LID and the group ID.

## Moderation Commands

- **!mod**

The main command to manage [moderation-based actions](moderation)

- **!warn**

Gives someone a warning: `!warn <@user|number> [reason]`. At the limit the bot does whatever the [warn settings](moderation#warnaction) say.

- **!warnings**

Lists the warnings in the group, or one person's.

- **!unwarn**

Takes a warning off someone. Add `all` to clear them.

- **!ban**

Makes the bot ignore someone in this group, for a set time if you want: `!ban [@user|number] [duration]`.

- **!unban**

As the name implies, it unbanns the person who was previously banned with `!unban [@user|number]`

- **!mute**

Locks the group so only admins can talk, for a set time if you want.

- **!unmute**

Unlocks the group.

- **!automute**

Mutes the group on a schedule: `!automute <once|all> <HH:MM>`, or `!automute off`.

- **!autounmute**

Unmutes the group on a schedule. Works like !automute.

- **!execute**

Kicks someone out of the group: `!execute <@user|number>`.

## Trusted Commands

These ones only work for trusted users.

- **!special**

A bunch of trusted extras. `!special join <group invite link>` and `!special leave <group id>` make the bot join or leave a group, and `!special listgroups` lists every group it is in. `!special addmember <number>` adds a number to the group you run it in, and `!special kickfrom <group id> <number>` removes a number from a group. `!special forceban <add|remove|list> [number]` bans a number from using the bot everywhere, and `!special debug` dumps some debug info (we dont talk about this).

- **!antiban**

Shows the anti-ban status and lets you change the rate limits. Use `!antiban banrisk` to check the ban risk and `!antiban reset` to reset it.

- **!messagedelay**

Changes how long the bot waits before sending a message: `!messagedelay set <min> <max>`, or `!messagedelay reset`.

- **!messagecooldown**

Changes how long people wait between commands: `!messagecooldown <normal> <heavy>`, or `!messagecooldown <on|off>`.

- **!bot**

Stops or resumes all sending from the bot with `!bot off` and `!bot on`.
