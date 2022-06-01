---
title: iRacing Reports Discord Bot - Welcome
---

# Welcome!

Thanks for supporting my iRacing Reports Discord Bot project.

To get the bot up and running in your Discord server you'll need to complete 4 steps:

1. Connect your Patreon account with iRacing Reports
2. Connect your Discord account with iRacing Reports
3. Invite the iRacing Reports Discord Bot to your Discord server
4. Create a role for the bot, and configure the required permissions

To begin the process, please open this following URL in a new tab:

[https://iracingreports.com/accounts/login](https://iracingreports.com/accounts/login)

## 1) Connect your Patreon

For the iRacing Reports systems to know that you're a supporter and what tier you're on, you'll need to use a system called OAuth to connect your Patreon account with the iRacing Reports website. For more information about OAuth, you can read this excellent explanation on the Patreon support site: https://www.patreon.com/portal/start/oauth-explained

Click the **CONNECT WITH PATREON** button:

![Connect with Patreon](https://user-images.githubusercontent.com/658935/171335957-9ab7a743-62cb-4445-a21d-fa60ff7fb8a9.png)

You'll enter the email address associated with your Patreon account and your password. Note, this information is sent to Patreon not us! You'll see that the URL is a patreon.com address.

![Log into Patreon](https://user-images.githubusercontent.com/658935/171336281-8f2d2996-1ef1-4d21-a142-83f0ed606739.png)

You'll be informed of the information that will be shared with us, click the **Allow** button.

![Patreon information](https://user-images.githubusercontent.com/658935/171336344-2a972b31-5fe3-4c67-a1b8-c407a6784646.png)

With this completed, you'll be returned to the iRacing Reports website and you should see the details of your Patreon account, along with what tier you're subscribed on and your payment status.

![Patreon connected](https://user-images.githubusercontent.com/658935/171336556-6459a95c-34e6-4aa0-8339-1611c26d999f.png)

## 2) Connect your Discord

To link up your Patreon account with your Discord account, you'll have to do a similar process with Discord.

Click the **CONNECT WITH DISCORD** button:

![Connect with Discord](https://user-images.githubusercontent.com/658935/171336907-e59ca607-da59-4fd1-9a53-e858d8230874.png)

You can either login using the email address associated with Discord and your password, or use the [QR Code Login](https://support.discord.com/hc/en-us/articles/360039213771-QR-Code-Login-FAQ) feature.

![Log into Discord](https://user-images.githubusercontent.com/658935/171337522-43854336-da32-499c-8d1f-8b44def7f44d.png)

You'll be informed of the information that will be shared with us, click the **Authorize** button.

![Discord information](https://user-images.githubusercontent.com/658935/171337604-5136f4d9-74db-4ee1-972a-5d5f18110e42.png)

With this completed, you'll be returned to the iRacing Reports website and you should now also see the details of your Discord account.

## 3) Invite the bot

If you have an invite to use, you'll be shown the **INVITE BOT TO YOUR SERVER** button. Click it!

![Invite bot](https://user-images.githubusercontent.com/658935/171338240-36e1cf64-cb4e-4fca-919b-915af78944c9.png)

Select the server you want to invite the bot into, and click the **Continue** button.

![Select server](https://user-images.githubusercontent.com/658935/171338512-55015d56-8336-4eaf-9898-718f21fbae7c.png)

You'll be shown a list of the permissions that will be granted to the bot. Click the **Authorize** button.

![iracing-reports-bot-v3-9](https://user-images.githubusercontent.com/658935/171338560-0bbd7921-8251-42f7-b0fc-f6667a7b4059.png)

With this completed, the bot will appear in your server!

## 4) Create a role and set permissions

Many teams / communities will limit the bot to only respond to commands in a single (or few) channels. We recommend creating a role for the bot and configuring the permissions.

For information on how to do this, please see Discord's documentation:

[https://support.discord.com/hc/en-us/articles/206029707-Setting-Up-Permissions-FAQ](https://support.discord.com/hc/en-us/articles/206029707-Setting-Up-Permissions-FAQ)

The permissions that the bot's role will require in channels where you want it to be able to respond to commands are:

* View Channel
* Send Messages
* Embed Links
* Attach Files
* Add Reactions
* Read Message History

# Adding drivers to your team

Once you've got the bot all ready to go, you'll probably want to add drivers to your team. Drivers in the team list will automatically be highlighted in responses from the bot and announcements of their races can be enabled.

You will use the `/manage_team add` command to do this. You'll need to provide the driver name and color you'd like used for the highlights for this driver. There is also an option field to link this driver to a Discord user. Be sure to select the Discord user from the auto complete list. It needs to resolve out to the purple text version.

![Add driver](https://user-images.githubusercontent.com/658935/171341212-42ddd9e3-c2e1-4fe5-8151-088f48052b67.png)
