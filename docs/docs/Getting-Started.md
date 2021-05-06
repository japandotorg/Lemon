## 💛 Is Lemon the right bot for your server?
### Lemon is probably a useful bot for your server if:
- ✅ Your server is active and needs automatic management/moderation
- ✅ You want to give more power to your moderators
- ✅ You need a warning system with auto-punishment system
### Lemon is probably NOT the right bot for your server if:
- ❌ You aren't willing to learn how to use Lemon using this wiki or the dynamic help menu Lemon has
- ❌ You aren't able and willing to read this wiki to solve most problems
- ❌ You don't fully trust your moderators
- ❌ You and/or your mods don't have a solid understanding of English

If any of the above apply, then Lemon will probably not be the best bot for your server, and you should consider searching on [top.gg](https://www.top.gg) for a different multi-purpose bot.

## 💛 Requirements
There are some light requirements for using Lemon. These requirements are in place to help save resources. Your server must meet all of the requirements below, or Lemon might automatically leave your server.
* **40 or more human members** - Lemon is a multipurpose moderation bot, and if you have fewer than 40 people, why do you need a bot to moderate anything?
* **More humans than bots** - Adding a lot of bots to a server just wastes resources, and making 'bot collection' servers is generally frowned upon. No server should need more bots than humans.
* **Strong knowledge of Discord and Discord bots, and the ability to read documentation** - Lemon is easy-to-use for admins and moderators, but only if they are willing to put in the time to read the documentation (this wiki). In general, asking for support for a question answered here will result in being redirected back to this wiki.
* **Follow Discord's Terms of Service** - While not automatically detected, if a server is reported for ToS violations, Vortex may be manually removed.
> ⚠ **Please read these requirements; Lemon may automatically leave your server if it does not meet them!**

## 💛 Adding Lemon to Your Server
The first step is to make sure that Lemon is actually on your server! To add a bot to your server, you must have the **Manage Server** permission on the server. If you do, you can click this link to add Lemon to your server:

> ⚠ **Please read the requirements above this section; Lemon may automatically leave your server if it does not meet the requirements**

[**Click here to invite Lemon**](https://discordapp.com/oauth2/authorize?client_id=807296190499913738&permissions=500559086&scope=bot)

If your server isn't listed, make sure you are correctly logged in by visiting https://discordapp.com/login

## 💛 Check Lemon's Permissions
For Lemon to operate correctly, it needs the permissions to be able to complete necessary tasks. The easiest way to achieve this is to give the `Lemon` role the Administration permission and drag it to the top (or near the top) of the role list, like so: 

> ![RoleOrder](https://i.imgur.com/MD4iyXg.gif)

## 💛 Setting up Lemon

The next step is configuring vortex for your server! You can type `c!helpadmin1` and `c!helpadmin2` to see the full list of settings commands, You can change the default `c!` prefix to anything you like if you don't like the default prefix by simply doing a `c!setprefix <newprefix>`. Don't worry if you forget the custom prefix you setup for the bot you can just @mention Lemon and type `@lemon prefix` and the bot will remind you the prefix you setup for your server. You can also check out the [[Full Command Reference|Commands]] to see what Lemon has to offer.

### Muted Role
The Muted role is the role that (usually) can be applied to a user to prevent them from sending messages, adding reactions, speaking, and connection to voice channels. If you don't already have a Muted role you can create a Muted role in the role settings of the server with the permissions of your liking and add them to the channels (I'll soon add a setup feature so that people don't have to set it up manually), if you already have a Muted role you can `c!setmuterole <rolename>` to setup the Muted role, Lemon should be able to set it up automatically, but if she doesn't be sure to set it up manually with the command given above.

### Logs
Lemon has various logs to keep track of different kinds of server activity. All commands for logs are found in the Admin commands, available via `c!helpadmin1` and `c!helpadmn2` or in the [[Full Command Reference|Commands]]. If your server is using the [[Warn system|Warns]], it is recommended to enable (at minimum) the ModLog.

### Moderator Role
The Moderator Role is a role that allows a user with said role to use all Moderation commands. The full list of Moderation commands is available via `c!helpmod` as well as on the [[Full Command Reference|Commands]]. To set a role to be the Moderator role, use `c!setmodrole <rolename>` (for example, if your moderator role is called "Staff", you'd run `c!setmodrole @Staff`). To disable the Moderator role, run `c!setmodrole none`. 

If no Moderator role is set, Moderation commands can only be run if the user has sufficient permissions natively (they would only be able to kick or ban someone with Lemon, if they could ban them via the Discord client as well).

Also, make sure to check out the [[Moderator Guide]] for helpful tips for moderating with Lemon!

### Auto-Mod
For full information about the Auto-Mod and its features, check out the [[Auto-Moderation]] page. You can check the default Auto-Mod settings using `c!helpamin1` or `c!helpadmin2`.