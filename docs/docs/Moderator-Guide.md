This is a guide for how to moderate a server using **Lemon**

## 🔨 Introduction
Lemon has all the tools that you need to moderate effectively and efficiently. The first thing you'll want to do is check out what prefix Lemon is using on your server. You can always use the `@lemon` mention and use `@lemon prefix` to see if the server has an custom prefix set (If you can't use the `@lemon` callback , ask your admin or server owner if the bot has all the permission it needs to use the moderation commands or just sending message permission in channels) Also check out the [[Moderation Commands section in the Full Command Reference|Commands#-moderation-commands]]

## 🔨 Moderation Commands
### Kick, Ban, Softban, Mute
All of these commands are very straightforward. The syntax for each is `c!command <@user/ID> [time] [reason]`. All of these can be used with IDs instead of mentions if you prefer. Muting support time aspects such as seconds (s), minutes (m) and hours (h), and users will automatically be unmuted after the amount of time has passed. The reason is optional but highly recomended as it will be used in both Discord's Audit Log as well as Lemon's Moderation Log.

Examples:
```
c!kick @inthdark.org Trolling
c!kick 759180080328081450 Trolling
c!mute @inthedark.org 10h Talks too much
c!mute 759180080328081450 10h Talks too much
c!softban @inthedark.org Toxic
c!softban 759180080328081450 Toxic
c!ban @inthedark.org Profanity ban
c!ban 759180080328081450 Profanity ban
```

### Cleaning Messages
Lemon's has two types of cleaning command right now, but I'll add more filters soon. One of the cleaning command is `c!purge` and the other one is `c!purgebot`. You can only delete 2-100 messages with this command, there is no default so you'll have to mention the number every time you want use this command, and also remember that clearing messages older than 14 days is not possible as that is a rule set by discord developers themselves.
There are some parameters for both commands that you can use, multiple parameters can be used at once. Running the command with 2 parameters is the same as running the command twice, each with one of those parameters.

* Purge Command 
   * Deletes the specified amount of messages from the provided channel. If no channel is given, the messages will be deleted from the current channel. If a member is provided, only their messages will be deleted from the chat.
   * Usage:
     ```
     c!purge [#channel/ID] <@user/ID> [message count] [reason]
     ```
   * Examples: 
     ```
     c!purge 20
     c!purge #general 10
     c!purge @inthedark.org 50
     c!purge #general @inthedark.org Toxic
     ```
* Purgebot Command 
   * Shifts through the specified amount of messages in the provided channel and deletes all bot commands and messages from Lemon. If no channel is given, the messages will be deleted from the current channel. No more than 100 messages may be deleted through at a time. Messages older than 2 weeks old cannot be deleted. 
   * Usage:
     ```
     c!purgebot [channel/ID] <message count> [reason]
     ```
   * Examples:
     ```
     c!purgebot 10
     c!prgebot #general 10
     ```

### Managing Warns
Some servers may heavily use the warning system, and others may not. Check with an admin or the server owner on the preference for using or not using the warn system. Check out the [[Warns]] page for a full explanation of how warns work!

### Using Slowmode
With Lemon, mods can enable slowmode for 0-59 seconds. If no channel is provided, then slowmode will affect the current channel. Provide a rate of 0 to disable.
* Usage:
  ```
  c!slowmode [channel/ID] <rate> [reason]
  ```
* Examples:
  ```
  c!slowmode 3
  c!slowmode #general 5
  ```

## 🔨 The Moderation Log
The moderation log is a channel that keeps track of all moderator actions taken within the server. This log will track bans, unbans, softbans, mutes, unmutes, timed mutes, kicks, cleaned messages, and warns, even if you don't use Lemon to perform the actions! When possible, make sure to provide reasons for all actions to keep the server organized!

## 🔨 Reasons
When banning or kicking someone with the Discord client, you're given a box in which to type a reason. Additionally, Lemon's commands support reasons for the actions that you may perform with them. However, sometimes you might not have time to write out a reason, and when the action gets put in the moderation log, it says `[no reason specified]`.