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

To begin the process, please open the following URL in a new tab:

## [https://iracingreports.com/accounts/login](https://iracingreports.com/accounts/login)

## 1) Connect your Patreon

For the iRacing Reports systems to know that you're a supporter and what tier you're on, you'll need to use a system called OAuth to connect your Patreon account with the iRacing Reports website. For more information about OAuth, you can read this excellent explanation on the Patreon support site: [https://www.patreon.com/portal/start/oauth-explained](https://www.patreon.com/portal/start/oauth-explained)

Click the **CONNECT WITH PATREON** button:

![1-connect-patreon](https://user-images.githubusercontent.com/658935/171343965-7e969b08-43d6-42c1-acb2-e9b4ebd3a0f4.png)

You'll enter the email address associated with your Patreon account and your password. Note, this information is sent to Patreon not us! You'll see that the URL is a patreon.com address.

![2-patreon-login](https://user-images.githubusercontent.com/658935/171344016-b9ce5312-8468-4e09-a74c-6a300e29d27d.png)

You'll be informed of the information that will be shared with us, click the **Allow** button.

![3-patreon-info](https://user-images.githubusercontent.com/658935/171344050-6e70bd2b-1733-4a9f-8c2e-abf2be4c31ef.png)

With this completed, you'll be returned to the iRacing Reports website and you should see the details of your Patreon account, along with what tier you're subscribed on and your payment status.


## 2) Connect your Discord

To link up your Patreon account with your Discord account, you'll have to do a similar process with Discord.

Click the **CONNECT WITH DISCORD** button:

![4-connect-discord](https://user-images.githubusercontent.com/658935/171344566-bbf9519a-df36-429e-abda-f5adb6c4f7ce.png)

You can either login using the email address associated with Discord and your password, or use the [QR Code Login](https://support.discord.com/hc/en-us/articles/360039213771-QR-Code-Login-FAQ) feature.

![6-discord-login](https://user-images.githubusercontent.com/658935/171344115-5cdfd007-285f-446f-95fa-7cb17b00c14b.png)

You'll be informed of the information that will be shared with us, click the **Authorize** button.

![7-discord-info](https://user-images.githubusercontent.com/658935/171344128-84cecc63-fa59-4e50-81f2-8e3a16b6efe8.png)

With this completed, you'll be returned to the iRacing Reports website and you should now also see the details of your Discord account.


## 3) Invite the bot

If you have an invite to use, you'll be shown the **INVITE BOT TO YOUR SERVER** button. Click it!

![8-invite-bot](https://user-images.githubusercontent.com/658935/171344148-e537d881-1e63-4e97-952e-09b28bb53faa.png)

Select the server you want to invite the bot into, and click the **Continue** button.

![9-select-server](https://user-images.githubusercontent.com/658935/171344164-38406048-2293-45e4-bd5c-cbb7a596fbb3.png)

You'll be shown a list of the permissions that will be granted to the bot. Click the **Authorize** button.

![10-bot-perms](https://user-images.githubusercontent.com/658935/171344180-d1da031d-74f8-4467-9500-0e94843ef186.png)

With this completed, the bot will appear in your server!


## 4) Create a role and set permissions

Many teams / communities will limit the bot to only respond to commands in a single (or few) channels. We recommend creating a role for the bot and configuring the permissions.

For information on how to do this, please see Discord's documentation:

[https://support.discord.com/hc/en-us/articles/206029707-Setting-Up-Permissions-FAQ](https://support.discord.com/hc/en-us/articles/206029707-Setting-Up-Permissions-FAQ)

The permissions that the bot's role will require in channels where you want it to be able to respond to commands are:

* View Channel
* Send Messages
* Send Messages in Threads
* Create Public Threads
* Embed Links
* Attach Files
* Add Reactions
* Read Message History


# Adding drivers to your team

Once you've got the bot all ready to go, you'll probably want to add drivers to your team. Drivers in the team list will automatically be highlighted in responses from the bot and announcements of their races can be enabled.

You will use the `/manage_team add` command to do this. You'll need to provide the driver name and color you'd like used for the highlights for this driver. There is also an option field to link this driver to a Discord user. Be sure to select the Discord user from the auto complete list. It needs to resolve out to the purple text version.

Below is an example of what a completely filled out command looks like:

![Add driver](https://user-images.githubusercontent.com/658935/171341212-42ddd9e3-c2e1-4fe5-8151-088f48052b67.png)




