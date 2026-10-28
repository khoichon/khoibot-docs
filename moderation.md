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

## antibadwordnosay

Same as antibadword, but the bot never says anything in the chat. It only deletes the message.

Values: `true` or `false`

Default: `false`

## antibadwordreport

Adds an "if this is incorrect, please report it" line to the bot's moderation message.

Values: `true` or `false`

Default: `false`

## casinoenabled

Controls whether the casino games (blackjack and slots) can be played in the group chat. This is separate from gamesEnabled.

Values: `true` or `false`

Default: `false`

## enablehelpmenu

Turns the help menu on for this group chat.(Theres a little secret :eyes:)
Values: `true` or `false`

Default: `false`

## toggleai

Controls whether !ai works in the group chat.

Values: `true` or `false`

Default: `true`

## trustedonly

When this is on, only trusted people and group admins can use the bot in the group chat.

Values: `true` or `false`

Default: `false`

## menudeletetime

How many seconds the !mod menu stays in the chat before the bot deletes it. 0 disables this fucntion.

Values: `0` or a number from `15` to `60`

Default: `15`

## disablelinking

Deletes messages with links in them. By default every link gets blocked, use linkblocklist to only block certain sites.

Values: `true` or `false`

Default: `false`

## disablelinkingnosay

Same as disablelinking, but the bot never says anything in the chat.

Values: `true` or `false`

Default: `false`

## linkblocklist

The websites to block when linking is disabled. If it is empty, every link gets blocked. Subdomains count as the main website.

Values: `add`, `remove` or `clear`, then a domain: `!mod linkblocklist add example.com`

Default: `empty`

## linkwhitelist

Websites that never get blocked, even if the blocklist (or the block everything rule) would catch them.

Values: `add`, `remove` or `clear`, then a domain

Default: `empty`

## linkexempt

Lets group admins and trusted people post links even when linking is disabled.

Values: `true` or `false`

Default: `false`

## warntoggle

Turns the [warn commands](commands) on or off in the group chat.

Values: `true` or `false`

Default: `true`

## warntrusted

Controls whether trusted people and group admins can be warned.

Values: `true` or `false`

Default: `true`

## warnlimit

How many warnings someone can get before the bot does the warnaction.

Values: a number from `1` to `20`

Default: `3`

## warnaction

What the bot does when someone reaches the warnlimit. You can use them together.

Values: `kick`, `ban [duration]` and `notify` (it just announces it), in any mix

Default: `notify`

## warnexpiry

Warnings older than this many days stop counting. 0 means they never expire.

Values: a number of days, or `0`

Default: `0`

## warncurses

How many curse messages the bot has to delete within the warncursestime window before the person gets a warning. 0 turns it off.

Values: a number from `0` to `50`

Default: set by the bot owner/hoster

## warncursestime

How many minutes the warncurses window lasts.

Values: a number of minutes from `1` to `60`

Default: set by the bot owner/hoster
