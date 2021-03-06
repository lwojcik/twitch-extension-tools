# twitch-extension-tools

A quick and dirty set of useful commands to simplify Twitch extension maintenance process. Built with [Vorpal](https://vorpal.js.org/).

## Prerequisites

* Node.js (preferably LTS version)
* Twitch API key (Client ID) - to obtain it go to https://dev.twitch.tv/ and register a new application
* Command line :-)

## Setup

* Edit `config.js` and add your Twitch API key as a value of `clientID` property
* Install the dependencies:
  ```npm install```

## Usage

* `npm start` - launch a CLI interface

Available commands:

* `getUserIds <twitchUsername1 twitchUsername2...>` or `gids <twitchUsername1 twitchUsername2...>` - get user IDs from one or more Twitch usernames. It generates comma-separated list of Twitch IDs. It's useful for creating long lists of accounts permitted to test the extension during hosted testing phase or after the release.

   Example:
  
   ```
   twitch-extension-tools$ gids Lirik Summit1G Ninja DansGaming
   23161357, 26490481, 19571641, 7236692
   twitch-extension-tools$ 
   ```
## License

Licensed under MIT License. See [LICENSE](https://raw.githubusercontent.com/lukemsc/twitch-extension-tools/master/LICENSE) for more information.
