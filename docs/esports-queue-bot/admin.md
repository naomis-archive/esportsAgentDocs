# `admin` Command

The `admin` command is used by server admins to help manage the queue and ensure stats are being accurately reported.

## Parameters

| Name     | Type     | Description                                                                                       |
| -------- | -------- | ------------------------------------------------------------------------------------------------- |
| `action` | Required | The administrative action to take. Must be one of `blockuser`, `unblockuser`, or `statsoverride`. |
| `target` | Required | The user to target with the action, as an `@mention` or a Discord ID.                             |

## Examples

| Command                                   | Result                                                                                       |
| ----------------------------------------- | -------------------------------------------------------------------------------------------- |
| `eq!admin statsoverride @nhcarrigan`      | Resets _all_ game stats for the Discord user nhcarrigan.                                     |
| `eq!admin blockuser @nhcarrigan`          | Blocks the Discord user nhcarrigan from using any bot commands.                              |
| `eq!admin unblockuser 465650873650118659` | Removes the block from the Discord user nhcarrigan, allowing them to use bot commands again. |
