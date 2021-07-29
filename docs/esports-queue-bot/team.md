# `team` Command

The `team` command is used to manage your team for a given game.

## Parameters

| Name              | Type     | Description                                                                                      |
| ----------------- | -------- | ------------------------------------------------------------------------------------------------ |
| `game`            | Required | The game you want to manage a team for.                                                          |
| `action`          | Required | The action to take. Can be one of `create`, `add`, `remove`, `view`, `calculate`, and `disband`. |
| `teamName/player` | Required | Depending on the `action`, this will be your team name or an `@mention` of a Discord user.       |

## Examples

| Command                                 | Result                                                                     |
| --------------------------------------- | -------------------------------------------------------------------------- |
| `eq!team rocketleague create Rockstars` | Creates a Rocket League team named Rockstars.                              |
| `eq!team rl add @Ooigle`                | Adds Ooigle to your Rocket League team.                                    |
| `eq!team rl remove @nhcarrigan`         | Removes nhcarrigan from your Rocket League Team.                           |
| `eq!team rl view`                       | Shows your current Rocket League team roster.                              |
| `eq!team rl calculate`                  | Calculates your initial team ranking for the matchmaking system.           |
| `eq!team rocket-league disband`         | Deletes your team, releasing all players and removing your captain status. |
