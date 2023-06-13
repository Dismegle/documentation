# Introduction
Thank you for using our Discord bot! This documentation aims to provide a clear understanding of the bot's functionality and features to help moderators effectively manage user interactions. Please read the following sections to familiarize yourself with the bot's behavior.

# Matching
The bot facilitates matching between users in private and group chats based on certain criteria. The matching rules are as follows:

Private Chats:
- Users will only be matched with individuals whom they haven't had a conversation with in the last month.

Group Chats:
- Users will be matched with other participants if they haven't interacted with more than half of the users in the group.

# VC Button Spam
To maintain a smooth user experience, the bot has implemented a timeout mechanism for users who spam the voice channel (VC) buttons excessively. The timeout period is set to 5 minutes, triggered when a user joins a voice channel five or more times within a span of less than 10 seconds.

This measure helps prevent rate-limiting of our helper bots in order to keep the feature smooth and fast for everyone!

# #start-chatting channel
For admins, it is possible to change the start menu message at any time using the following command:

```arduino
/admin action:#start-chatting menu args:<your message>
```

However, it is recommended to keep the message short and sweet, with an emphasis on the four buttons. Too much text can confuse users and lead them to overlook the channel as just another information channel.

# Commands
The bot provides several commands to facilitate moderation tasks. Here are the available commands:

`/inf add @user <reason>`: Adds an infraction for a specific user, providing a reason for the infraction.

`/inf list @user`: Lists all infractions for a given user.

`/inf delete`: Deletes an infraction.

`/history @user`: Displays the chat history of a user, showing who they have interacted with.

`/current`: Shows the list of active chats.

`/stats members`: View statistics about member growth.

`/stats chats`: View statistics about chat activity.

`/stats waiting`: View statistics about wait times.
  
# Flagging
The bot includes flagging functionality to help identify problematic behavior. Here's how it works:

When a member uses a flagged keyword, it will appear in the #flagged-logs channel. Admins can then use the menu options to either assign a punishment or mark it as reviewed.
Punishments marked with the hammer emoji will result in an immediate ban, while those marked with the warning emoji will issue a warning before taking further action. If a user has multiple offenses for the same reason, they will be banned to maintain quality control.
Moderators can review flagged chats by using the /flag command. This command removes the member from the chat, allowing mods to read the conversation and identify any issues. Punishments can be assigned using /inf add accordingly.
If a flag appears to be without valid reason, the punishment reason "False Flag" can be used.
Once the flagged chat has been handled, moderators should close the thread using the "Close Thread" button to remove it from the channel list. The flagged chat will be archived indefinitely for future reference unless manually deleted.


# Conclusion
We hope this documentation provides you with a clear understanding of the bot's behavior and features. If you have any further questions or require assistance, please don't hesitate to reach out to our support team.

Thank you for using our Discord bot!
