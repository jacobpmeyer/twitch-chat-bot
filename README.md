# Twitch Chat Bot

This project is a simple Twitch chat bot built with Node.js and the `tmi.js` library. It connects to a Twitch channel and can respond to specific chat commands, starting with a basic `!dice` command that simulates rolling a dice.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- [Node.js](https://nodejs.org/) (if running locally without Docker)
- [Docker](https://www.docker.com/get-started) (for containerization)
- [Docker Compose](https://docs.docker.com/compose/install/) (for running multi-container Docker applications)

### Installation

#### Running Locally without Docker

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/twitch-chat-bot.git
   ```
2. Navigate to the project directory:
   ```bash
   cd twitch-chat-bot
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Create a `.env` file in the root directory with your Twitch credentials and channel name as described in the [Environment Variables](#environment-variables) section.

5. Run the bot:
   ```bash
   node bot.js
   ```

#### Running with Docker

1. Ensure Docker and Docker Compose are installed on your machine.
2. Clone the repository (if you haven't already):
   ```bash
   git clone https://github.com/yourusername/twitch-chat-bot.git
   ```
3. Navigate to the project directory:
   ```bash
   cd twitch-chat-bot
   ```
4. Create a `.env` file in the root directory with your Twitch credentials and channel name. This file will be automatically used by Docker Compose to set environment variables in your container.

5. Build and run the application using Docker Compose:
   ```bash
   docker compose up --build
   ```

This command builds the Docker image (if necessary) and starts the chat bot in a container. Your application is now running inside a Docker container and connected to Twitch using the credentials provided in the `.env` file.

## Environment Variables

To run this project, you need to add the following environment variables to your `.env` file:

- `BOT_USERNAME`: The username of your Twitch bot account.
- `OAUTH_TOKEN`: The OAuth token for authenticating your Twitch bot account. Generate this token at [TwitchApps TMI](https://twitchapps.com/tmi/).
- `CHANNEL_NAME`: The name of the Twitch channel your bot will join.

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
