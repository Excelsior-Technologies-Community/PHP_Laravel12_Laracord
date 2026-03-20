# PHP_Laravel12_Laracord


## Project Description

PHP_Laravel12_Laracord is a Discord bot project built with Laravel 12.
It demonstrates how to integrate a Discord bot using Laracord, a Laravel-based framework for creating Discord bots easily.

The project provides a working bot that can respond to commands like !ping and !help, and can be extended with custom commands and interactions. It’s a perfect starting point for developers who want to combine Laravel’s power with Discord bot development.



## Features

- Connects a Laravel application to Discord using Laracord.

- Supports custom bot commands (e.g., !ping, !help).

- Easy configuration via .env file for bot token and command prefix.

- Console logs to monitor bot status and commands.

- Extendable for additional features like moderation, music, or games.

- Fully compatible with Laravel 12 and PHP 8.2+.




## Technologies Used

- PHP 8.2 – Core programming language

- Laravel 12 – Backend framework for structured application

- Laracord – Laravel package to create Discord bots

- Composer – Dependency manager for PHP

- Discord API – Platform to interact with Discord servers



---



## Installation Steps


---


## STEP 1: Create Laravel 12 Project

### Open terminal / CMD and run:

```
composer create-project laracord/laracord PHP_Laravel12_Laracord

```

### Go inside project:

```
cd PHP_Laravel12_Laracord

```

#### Explanation:

Installs a fresh Laravel 12 project with Laracord pre-configured.

cd moves you into the project folder to start working.




## STEP 2: Configure Your Bot Token

### Get a valid Discord bot token:

1. Go to Discord Developer Portal

2. Create a new application.

3. Go to Bot → Add Bot → Copy the Bot Token.

4. Open the .env file in your project folder and add:

```
DISCORD_TOKEN=PASTE_YOUR_BOT_TOKEN_HERE
DISCORD_COMMAND_PREFIX=!

```

#### Explanation:

.env stores secret keys like your Discord bot token.

DISCORD_COMMAND_PREFIX sets the prefix for bot commands.





## STEP 3: Run the Bot

### From your project folder, run:

```
php laracord

```

### If everything is set up correctly, you should see logs like:

```
Client is ready.
Successfully booted Laracord with 2 commands, and 1 interaction.
+---------+------------------------+
| Command | Description            |
+---------+------------------------+
| !ping   | Ping? Pong!            |
| !help   | View the command help. |
+---------+------------------------+

```

#### Explanation:

Starts the bot and connects it to Discord.

Shows available commands and confirms the bot is online.





## STEP 4: Invite the Bot to Your Server

1. Copy the OAuth2 link shown in the logs after running php laracord.

2. Open it in your browser and select a server you manage.

3. Authorize the bot to join the server.


#### Explanation:

Adds your bot to a Discord server so it can interact with users.




## STEP 5: Test the Bot

### In your Discord server, type:

```
!ping

```

### The bot should respond with:

```
Pong!

```

#### Explanation:

Confirms that the bot is working and responding to commands.



## Expected Output:

### Bot Console Logs:


<img src="screenshots/Screenshot 2026-03-20 172054.png" width="900">


### OAuth2 Authorization:


<img src="screenshots/Screenshot 2026-03-20 175121.png" width="900">



---

## Project Folder Structure:

```
PHP_Laravel12_Laracord/
├── app/
├── laracord/          # Bot commands & events
├── config/
├── database/
├── public/
├── resources/
├── routes/
├── storage/
├── tests/
├── vendor/
├── .env
├── artisan
└── composer.json

```
