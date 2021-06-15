# `notification` Command

This command is used to manage the notification messages for the server. Depending on the `action`, the behaviour of the command changes.

## Parameters

| Name     | Type     | Description                                                                                            |
| -------- | -------- | ------------------------------------------------------------------------------------------------------ |
| `action` | Required | The action to take with the notification system. Must be one of `create`, `view`, `delete`, or `help`. |

### When `action` is `create`

The `create` action is used for creating a new notification, and takes the following parameters:

| Name      | Type     | Description                                                                                |
| --------- | -------- | ------------------------------------------------------------------------------------------ |
| `channel` | Required | The Discord channel the notification should be posted in. Format this as a `#channel` tag. |
| `time`    | Required | The time, in minutes, to wait before sending the notification again.                       |
| `message` | Required | The message the notification should contain.                                               |

### When `action` is `view`

The `view` action will allow you to view a list of active notifiations. Optionally pass a notification number to see that notification's details.

| Name     | Type     | Description                                            |
| -------- | -------- | ------------------------------------------------------ |
| `number` | Optional | The number of the notification you would like to view. |

### When `action` is `delete`

The `delete` action is used to delete notifications.

| Name     | Type     | Description                               |
| -------- | -------- | ----------------------------------------- |
| `number` | Required | The number of the notification to delete. |

### When `action` is `help`

No additional parameters are available.

## Examples

| Command                                                    | Result                                                                                                                                |
| ---------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| `!esports notification help`                               | Displays an embed with information on how to use the notification system.                                                             |
| `!esports notification create #general 30 Hello everyone!` | Will create a new notification for the general channel. The notification will post every 30 minutes, with the text "Hello everyone!". |
| `!esports notificaiton view`                               | View a list of server notifications, including the notification number.                                                               |
| `!esports notification view 1`                             | View specific details on notification number 1.                                                                                       |
| `!esports notification delete 1`                           | Delete notification number 1. The bot will stop posting it.                                                                           |
