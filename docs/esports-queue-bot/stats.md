# `stats` Command

The `stats` command is used to set your rank for a specific game mode in a game. You must register your stats in order to join the queue for that game mode.

## Parameters

| Name       | Type     | Description                                                 |
| ---------- | -------- | ----------------------------------------------------------- |
| `game`     | Required | The game you want to set stats for.                         |
| `gameType` | Required | The type of game you are setting stats for.                 |
| `rank`     | Required | Your rank in that game type from the provided stat tracker. |

## Examples

| Command                          | Result                                                                |
| -------------------------------- | --------------------------------------------------------------------- |
| `eq!stats rocketleague 1v1 1000` | Sets your rank to `1000` for the Ranked Solo mode in Rocket League.   |
| `eq!stats rl 3v3 12`             | Sets your rank to `12` for the Ranked Standard mode in Rocket League. |
