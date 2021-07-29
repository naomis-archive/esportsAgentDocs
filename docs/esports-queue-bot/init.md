# `init` Command

The `init` command is used to set up your initial profile for a supported game. You must do this before the `stats` command is available to you.

## Parameters

| Name       | Type     | Description                                            |
| ---------- | -------- | ------------------------------------------------------ |
| `game`     | Required | The game you want to set up your profile for.          |
| `platform` | Required | The platform code you want to set up your profile for. |
| `username` | Required | Your username on the specified platform.               |
| `rank`     | Required | Your current rank from the approved tracking service   |

## Examples

| Command                                      | Result                                                                       |
| -------------------------------------------- | ---------------------------------------------------------------------------- |
| `eq!init rocketleague steam nhcarrigan 2000` | Sets up your Rocket League profile as the user nhcarrigan on Steam.          |
| `eq!init rl psn notnhcarrigan 1000`          | Sets up your Rocket League profile as the user notnhcarrigan on PlayStation. |
