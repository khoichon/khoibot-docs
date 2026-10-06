# Moderation

khoibot has tools that can help with moderating Group Chats with a key-value based settings system.

The settings below are the chapter names.

To set a value of a key, use `!mod <key> <value>`


## antibadword

Turns on the bot's moderation system. Requires the bot owner to run the moderation submodule with the bot.

Values: `true` or `false`

Default: `false`

## badwordlog

Shows how much information the bot will show in its moderation message.
- `silent`: Please be nice. 
- `info`: Please be nice. Toxicity score: `average score`.
- `debug`: Please be nice. Debug: `every toxicity category ranked from highest score to lowest score`

Values: `silent`, `info` or `debug`

Default: `info`

## welcomeMsgEnabled

Controls if the welcome message is enabled in a group chat.

Values: `true` or `false`

Default: `false`

## welcomeMsg

The message shown when a new member joins a group chat (if enabled).

Placeholders: `[user]` -> The user who joined.

Values: `string`

Default: `Welcome to the group, [user]!`

## gamesEnabled

Controls whether games are enabled in the group chat.

Values: `true` or `false`

Default: `true`