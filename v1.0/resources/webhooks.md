---
title: "Use the Microsoft Graph API to get change notifications"
description: "The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes. For more details, including how to subscribe to and handle incoming notifications, see Set up notifications for changes in user data."
localization_priority: Priority
author: "baywet"
ms.prod: ""
doc_type: conceptualPageType
---

# Use the Microsoft Graph API to get change notifications

The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive notifications. Client apps use notifications to update their state upon changes. For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).

Using the Microsoft Graph API, an app can subscribe to changes on the following resources:

| **Resource** | **Supported resource paths** | **Resource data can be included in notifications**                  |
|:----------------|:------------|:-----------------------------------------|
| Outlook [message][] | Changes to all messages in a user's mailbox: <br>`/users/{id}/messages`<br>Changes to messages in a user's Inbox:<br>`/users/{id}/mailFolders('inbox')/messages` | No |
| Outlook [event][] | Changes to all events in a user's mailbox:<br>`/users/{id}/events` | No |
| Outlook personal [contact][] | Changes to all personal contacts in a user's mailbox:<br>`/users/{id}/contacts` | No |
| [user][] | Changes to all users:<br>`/users` <br>Changes to a specific user:<br>`/users/{id}`| No |
| [group][] | Changes to all groups:<br>`/groups` <br>Changes to a specific group:<br>`/groups/{id}` | No |
| Office 365 group [conversation][] | Changes to a group's conversations:<br>`groups/{id}/conversations` | No |
| [driveItem][] on OneDrive (personal) | Changes to content within the hierarchy of _any folder_:<br>`/users/{id}/drive/root` | No |
| [driveItem][] on OneDrive for Business | Changes to content within the hierarchy of the _root folder_:<br>`/drives/{id}/root`<br> `/users/{id}/drive/root` | No |
| Security [alert][] | Changes to a specific alert:<br>`/security/alerts/{id}` <br>Changes to filtered alerts:<br> `/security/alerts/?$filter`| No |
| Teams [chatmessage](/graph/api/resources/subscription?view=graph-rest-beta) | Changes to chat messages in all channels in all teams:<br>`/teams/allMessages` <br>Changes to chat messages in a specific channel:<br>`/teams/{id}/channels/{id}/messages`<br>Changes to chat messages in all chats:<br>`/chats/allMessages` <br>Changes to chat messages in a specific chat:<br>`/chats/{id}/messages` | Yes |

> **Note**: Any resource path that begins with `/users/{id}` can also accept `/me` to reference the signed-in user.

## Permissions

In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.

| Permission type                        | Supported resource types                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| Delegated - work or school account     | [alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]|
| Delegated - personal Microsoft account | [contact][], [driveItem][], [event][], [message][]                                        |
| Application                            | [alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]|


## See also

- [Subscription resource type](./subscription.md)
- [List subscriptions](../api/subscription-list.md)
- [Get subscription](../api/subscription-get.md)
- [Create subscription](../api/subscription-post-subscriptions.md)
- [Update subscription](../api/subscription-update.md)
- [Delete subscription](../api/subscription-delete.md)

[contact]: ./contact.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
