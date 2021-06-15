# `queue` Command

The `queue` command is used to join a queue for the specific game mode. When you join the queue, if our algorithm finds a match both you and the other player will be notified.

## Parameters

| Name       | Type     | Description                                    |
| ---------- | -------- | ---------------------------------------------- |
| `game`     | Required | The game you want to queue for.                |
| `gameType` | Required | The game type, or mode, you want to queue for. |

## Examples

| Command                     | Result                                                                   |
| --------------------------- | ------------------------------------------------------------------------ |
| `eq!queue rocketleague 1v1` | Adds you to the queue for the Ranked Solo game mode in Rocket League.    |
| `eq!queue rl 2v2`           | Adds you to the queue for the Ranked Doubles game mode in Rocket League. |
