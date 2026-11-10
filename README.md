# Telegram Bot – DAO Announcement Bot

A Node.js-based Telegram bot designed to assist with group management and announcement-related activities. It automates welcome messages for new members and provides basic bot commands for user support and interaction.

## Features

- **Welcome Messages** – Automatically welcomes new members when they join a Telegram group.
- **Bot Introduction** – Provides a welcome message when users execute `/start`.
- **Support Command** – Displays bot usage information through `/support`.
- **Real-Time Message Handling** – Uses Telegram polling to listen for incoming messages and events.
- **Group Integration** – Supports integration with Telegram group chats.

## Tech Stack

- **Runtime:** Node.js
- **Language:** JavaScript
- **Library:** node-telegram-bot-api
- **Platform:** Telegram Bot API

## Available Commands

| Command | Description |
|---|---|
| `/start` | Displays the bot's welcome message. |
| `/support` | Displays available commands and support information. |

## Getting Started

### Prerequisites

- Node.js and npm installed.
- A Telegram account.
- A Telegram Bot Token generated through [@BotFather](https://t.me/BotFather).

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/elfreddev/Telegram-Bot.git
   ```

2. Navigate to the project directory:

   ```bash
   cd Telegram-Bot
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Create a `.env` file in the project root:

   ```env
   TELEGRAM_BOT_TOKEN=your_telegram_bot_token
   ```

5. Install dotenv:

   ```bash
   npm install dotenv
   ```

6. Update `bot.js` to load the environment variable:

   ```javascript
   require('dotenv').config();

   const token = process.env.TELEGRAM_BOT_TOKEN;
   ```

7. Start the bot:

   ```bash
   node bot.js
   ```

## Project Structure

```text
Telegram-Bot/
├── bot.js
├── main.html
├── package.json
├── package-lock.json
├── .env
└── .gitignore
```

## Configuration

The bot uses a Telegram Bot Token to authenticate with the Telegram Bot API.

Keep your credentials secure:
- Store tokens in environment variables.
- Never commit `.env` files.
- Add `.env` to `.gitignore`.
- Regenerate exposed bot tokens through BotFather.

## Future Enhancements

- Custom announcement creation and management.
- `/setannouncement` command implementation.
- `/deleteannouncement` command implementation.
- Scheduled group announcements.
- Admin-only command permissions.
- Custom Telegram keyboards and interactive buttons.
- Database integration for storing announcements.

## License

This project is licensed under the ISC License.
