# What are ponts?
Points are like leveling system that users accumulate for engaging in your server.

## How do I earn points?
You can earn points by sending messages, by using Lemon's commands, and by spending time in voice chat. And if someone's feeling generous, they can give you points by using the `c!givepoints <@user/ID>` command. Here is the default point's per action list:
```
    Message Points :: 1 per message
    Command Points :: 1 per command
    Voice Points   :: 1 per minute
```
To quickly see your server's points per action again, you may use the command `c!pointsper` 

## How do I check how many points/position I have?
* You can use `c!leaderboard` to check the server's present cycle's leaderboard.
* You can use `c!points` to check how many points you have in the present cycle and `c!points <@user/ID>` to check anyone else's points.
    * Examples:
    ```
    c!points @inthedark.org
    c!points 759180080328081450
    ```
* You can use `c!position` to check what position you have in the present cycle and `c!position <@user/ID>` to check someone else's position.
    * Examples:
    ```
    c!position @inthedark.org
    c!position 759180080328081450
    ```
* You can use `c!totalpoints` to check your total points in the server and `c!totalpoints <@user/ID>` for someone else's total points.
    * Examples:
    ```
    c!totalpoints @inthedark.org
    c!totalpoints 759180080328081450
    ```

## Can I change the points someone recieves per message/command/minute in voice?
* Set the amount of points earned per user message using `c!setmessagepoints`.
   * Usage:
   ```
   c!setmessagepoints <point count>
   ```
* Set the amount of points earned per Lemon's command used with `c!setcommandpoints`
   * Usage:
   ```
   c!setcommandpoints <point count>
   ```
* Set the amount of points earned per minute spent in voice chat using `c!setvoicepoints`
   * Usage:
   ```
   c!setvoicepoints <point count>
   ```

## What is The Crown?
If a crown role and crown schedule are set, then the person with the most points of that cycle will win! Additionally, everyone's points will be reset to 0 (total points will remain untouched).
If your server doesn't have the crown system setup then check with an admin or the server owner on the preference for using or not using the crown system.
> Below is a brief description about the crown system and most importantly how to set it up:
### Crown Role
The Crown role is an award that Lemon will give to the member with the most points each cycle.
* Usage: 
```
c!setcrownrole <@role/ID>
```
* Examples:
```
c!setcrownrole @Crowned
c!setcrownrole 806389896612282389
```

### Crown Message
Set the message Lemon will say during the crown role rotation. You may use ?member to substitute for a user mention, ?username to substitute for someone's username, ?tag to substitute for someone's full discord tag (username + tag), ?role to substitute for the Crown role and ?points to substitute for the current points of the winner. Enter no message  to clear the current crown message. A crown message will only be sent if a crown channel, crown role, and crown schedule are set.
* Usage:
```
c!setcrownmessage <message>
```
* Examples:
```
c!setcrownmessage ?member has won the ?role
c!setcrownmessage ?member has won the ?role, congrats ?username won with ?points points
```

### Crown Channel
Set the crown message text channel for your server. Provide no channel to clear the current crown channel. A crown message  will only be sent if crown channel, crown role, crown schedule are set.
* Usage:
```
c!setcrownchannel <channel/ID>
```
* Examples:
```
c!setcrownchannel #general
c!setcrownchannel 806755276753076224
```

### Crwon Schedule
Set the schedule for Lemon's Crown role rotation.
The format is [cron](https://crontab.guru/#)-style:
```
*    *    *    *    *
┬    ┬    ┬    ┬    ┬
│    │    │    │    │
│    │    │    │    └ day of week (0 - 7)
│    │    │    └───── month (1 - 12)
│    │    └────────── day of month (1 - 31)
│    └─────────────── hour (0 - 23)
└──────────────────── minute (0 - 59)
```
If you wish to use multiple values for any of the categories, please separate them with `,`. Step syntax is also supported, for example: `0 */1 * * *` (every hour). For the day of the week, both 0 and 7 may represented Sunday.
If you need additional help building your cron, please click [here](https://crontab.guru/#). Enter no schedule to clear the current crown schedule.
* A Crown role must also be set to enable role rotation.
* **Please Note:** To prevent potential Discord API abuse, minutes and seconds will always be set to 0.
* Usage:
```
c!setcrownschedule <cron>
```
* Examples:
```
c!setcrownschedule 0 21 * * 3,6
c!setcrownschedule 0 0 15 * 
```

***
### You can enable or disable Lemon's point tracking using `c!togglepoints`