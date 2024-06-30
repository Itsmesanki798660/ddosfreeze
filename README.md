# DDoS Attack Bot

### Installation

1. Clone the repository:
   git clone https://github.com/DvijK/ddosfreeze.git
   cd ddosfreeze

2. Install the required libraries:

   pip install telebot
   pip install flask
   pip install aiogram
   pip install pyTelegramBotAPI
   
### Configuration

1. Create a bot on Telegram and obtain your bot token.

2. Replace the placeholder token in the script with your actual bot token:

   ```python
   bot = telebot.TeleBot('YOUR_BOT_TOKEN')
   ```

3. Add your admin user IDs in the `admin_id` list:

   ```python
   admin_id = ["YOUR_ADMIN_ID"]
   ```

### Usage

1. Run the bot:

   ```sh
   chmod +x *
   python venom.py
   ```

2. Interact with the bot on Telegram using the available commands.

## Bot Commands

### User Commands

- `/start` - Welcome message.
- `/help` - Display help information and available commands.
- `/bgmi <target> <port> <time>` - Initiate a DDoS attack on the specified target.
- `/rules` - Display rules for using the bot.
- `/plan` - Display available plans and pricing.
- `/mylogs` - Show recent command logs for the user.
- `/myinfo` - Display user's information and approval status.

### Admin Commands

- `/add <userId> <duration>` - Add a user with a specified approval duration.
- `/remove <userId>` - Remove a user from the authorized list.
- `/allusers` - Display all authorized users.
- `/logs` - Display logs of all commands executed by users.
- `/clearlogs` - Clear the command logs.
- `/clearusers` - Clear the list of authorized users.
- `/broadcast <message>` - Send a broadcast message to all authorized users.

## File Structure

- `ddos_bot.py` - Main bot script containing all functionalities.
- `users.txt` - File to store allowed user IDs.
- `log.txt` - File to store command logs.
- `keep_alive.py` - Script to keep the bot running (e.g., for use with Repl.it).

Happy DDoS'ing responsibly! 🚀
