## What are warns?
Warns are points that users accumulate for misbehaving. Warns are often represented as warnings. Whenever a user receives warns, they are sent a private message detailing the amount and reason for their warns, they are automatically punished according to the server's settings!

## How do I give/take away warns?
To give someone warns, use the `c!warn` command. To remove strikes, use the `c!` command. The usage for these commands is as follows:
```
c!warn <@user/ID> [reason]
c!clearnwarns <@user/ID> [reason]
```
Examples:
```
c!warn @inthedark.org being rude
c!clearwarns @inthedark.org
```

## What is warnpurge?
Wans the specified member in your server and then purges their messages from the channels with the message count provided. The usage of this command is as follows:
```
c!warnpurge <@user/ID> <message count> [reason]
```
Examples: 
```
c!warnpurge @inthedark.org 50
c!warnpurge 759180080328081450 10 toxic
```
## Can I check the reasons and how many warns someone has?
Yes you can check how many warns someone has with their date and reason and you'll also be able to see who have warned the person with a specific warn count.
Usage:
```
c!warns <@user/ID>
```
Example:
```
c!warns @inthedark.org
c!warns 759180080328081450
``` 

## What is auto-kick?
With auto-kick enabled Lemon will automatically kick someone from your server who has the. Like if amount specified in auto-kick is after 4 warns, then the users will automatically get kicked out from your server after receiving 4 warns. You will have to setup auto-kick for using it. Provide no warn count or a warn count of 0 to disable auto-kick.
Usage:
```
c!setautokick <warn count>
```
Example:
```
c!setautokick 3
c!setautokick 0
```