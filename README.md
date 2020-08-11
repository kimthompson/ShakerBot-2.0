# ShakerBot

## Installation and Boot

Make sure you have installed Node, NPM and git. Once you've cloned this repo, run the command `npm i` to install all the required packages, then run `npm run build` to build the bundle. Run the command `npm run dev` to see it in action. `npm run start` runs a this bot in production mode.

## Commands

### Pinging Roles

**ShakerBot** only listens to the *bot-commands* channel on our server, and will delete any user's input as soon as it's entered in chat. Discord roles can be pinged by placing an "@" before a pingable role. This will let everyone tied to that role know that there's a message for them. For example:

```
@DPS: Any DPS need a quick queue?
```

The available roles to ping are:

* DPS
* Tank
* Healer

### Reminders/Alerts

We have also made a few roles to manage reminders and alerts for scheduled activities in-game. The following roles can also be pinged for organizing groups. Please note that these alerts send scheduled private messages at the listed times.

Weekly reminders for the Jumbo Cactpot drawing in the Gold Saucer(Saturdays at 8PM and 8:55PM Central)

```
!cactpot
```

Bi-weekly reminders for Khloe's Wondrous Tails journal (Tuesdays and Fridays at 6PM Central)

```
!journal
```

### Groups

Beyond the above roles for matchmaking, there are other activities that might not require a specific party makeup, but still require some planning. Use the following roles to help set up activities with like-minded players.

For running treasure maps, Aquapolis, Lost Canals:

```
!treasure
```

### Other commands

If you want a printout of your active roles sent to you, use the following command:

```
!roles
```

## COMING SOON

```
!hunt *creature*
```

```
!fate *fate name*
```

### Assigning Roles

Cannot reimplement these until we figure out how to make Shaker admin, or at least give him role assign authority. In order to do that, we need to set up TFA on his behalf. I don't want to even get into it right now, but here are the resources I was attempting to combine:

* https://discord.com/developers/docs/topics/oauth2#bots
* https://discordjs.guide/popular-topics/permissions-extended.html#discord-s-permission-system
* https://discord.js.org/#/docs/main/stable/class/GuildMemberRoleManager?scrollTo=remove
* Our permissions integer for `ADMINISTRATOR` should be 8. Where I shove that integer, idek.

Once you're comfortable with a given role and above level 50, type the corresponding role command to assign it to yourself. You can be in more than one if you'd like! The following commands are valid:

* `!tank`
* `!healer`
* `!dps`

To remove yourself from a role, simply run that role's command again. In this respect, it kind of works like a toggle.

### Main Roles

Use the following commands to set your main role, which will color your name within this channel. Thes are purely cosmetic, and cannot be pinged like other roles.

* `!tankmain`
* `!healermain`
* `!dpsmain`

If you feel like switching to another main role, simply type in the one that you want, and Shaker will remove you from the old one.

