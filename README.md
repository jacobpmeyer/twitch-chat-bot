# Twitch Chat Bot

This project is a simple Twitch chat bot built with Node.js and the `tmi.js` library. It connects to a Twitch channel and can respond to specific chat commands, starting with a basic `!dice` command that simulates rolling a dice.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Node.js
- npm

### Installation

1. Clone the repository:
```bash
git clone https://github.com/jacobpmeyer/twitch-chat-bot.git
```

2. Navigate to the project directory:
```bash
cd twitch-chat-bot
```

3. Install the project dependencies:
```bash
npm install
```

### Setup

1. Create a `.env` file in the root directory with the following content, replacing `your_value_here` with your actual data:
```bash
BOT_USERNAME=your_value_here
OAUTH_TOKEN=oauth:your_value_here
CHANNEL_NAME=your_value_here
```
See [Environment Variables](#environment-variables) section for more details.

2. Run the bot:
```bash
node bot.js
```

## Environment Variables

To run this project, you need to add the following environment variables to your `.env` file:

- `BOT_USERNAME`: The username of your Twitch bot account.
- `OAUTH_TOKEN`: The OAuth token for authenticating your Twitch bot account. Generate this token at [TwitchApps TMI](https://twitchapps.com/tmi/).
- `CHANNEL_NAME`: The name of the Twitch channel your bot will join.

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

- `tmi.js` library for providing an easy interface to Twitch's chat.
