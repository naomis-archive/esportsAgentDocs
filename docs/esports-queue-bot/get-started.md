# Getting Started

This page will walk you through how to begin using our service for your intended game. There are two sections - one for players, and one for team captains. Choose the section relevant to your role.

> [!TIP]
> For the best stat tracking and scrim finding experience, ensure that all of your team members have [joined our Discord server](_https://discord.gg/GB2HqBpvf9)

## For Players

As a player, your only responsibility is to provide the bot with your game details and current ranking.

To accomplish this, use the `init` command with the following format:

```txt
eq!init <game> <platform> <username> <rank>
```

So, if you wanted to identify yourself for Rocket League as nhcarrigan on Steam, you'd do:

```txt
eq!init rl steam nhcarrigan 2000
```

Note that once you've set your initial ranking you will not be able to change it. Please ensure the stat you provide matches your stat on the game's [approved tracker](/esports-queue-bot/supported-games.md). Our admin team will verify this as needed.

## For Captains

> [!NOTE]
> Ensure that all of your players have initialised their stats for your desired game, as documented above. **This includes you as the captain!**

These steps will walk you through setting up your team, adding players, and joining the queue.

The two commands you will need to use are the `team` and `queue` commands.

### Create Your New Team

If you have not used our service for a particular game, you will need to create your team first:

```txt
eq!team <game> create <teamName>
```

For example, if you wanted to create the team `nhcommunity` for Rocket League, you would use:

```txt
eq!team rocket-league create nhcommunity
```

This will create the team, mark you as the captain, and add you to the team's player list.

### Add Your Players

Next you need to add your players. For each player you want to add, do:

```txt
eq!team <game> add <@player>
```

Where `@player` is an `@mention` of the Discord user you want to add.

For example, to add oDEF to your new Rocket League team, you would use:

```txt
eq!team rocketleague add @oDEF
```

Note that the bot will not allow you to add more players than the game's configured maximum.

### Calculate Your Rank

> [!WARNING]
> This command can only be run **once**. Be sure you have added all of your intended players before running this command.

After you have added all of your players, you need to calculate your initial team ranking. This ranking will be used to find you compatible teams in the scrim service.

To calculate your initial rank, use:

```txt
eq!team calculate
```

The bot will generate your team's initial rank.

### Join the Queue

Congratulations! You are now ready to join the queue. To add your team to the queue for a given game:

```txt
eq!queue <game>
```

If you have configured your team correctly, the bot will add you to the queue. When a team is found in the queue at a similar skill level, you will be notified that your match is ready to start.

### Report a Win

In order to get the best matchmaking experience, it is important that you report your win after a match.

> [!NOTE]
> Keep your replays on hand for any match you report as a win. The Esports Agent team reserve the right to verify any win reported through our system.

To report a win, you need to know the Discord name of your opposing team's captain. Then:

```txt
eq!win <game> <@opponent>
```

To report a win against Vokul's Rocket League team:

```txt
eq!win rl @Vokul
```
