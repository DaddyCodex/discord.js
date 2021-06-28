# discord.js

![image](https://user-images.githubusercontent.com/79264000/123623342-4deb2d80-d7db-11eb-8bbb-cf02f8360c0a.png)

# How to install

```npm install discord.js```


# Example Usage

```const { Client, Intents } = require('discord.js');
const client = new Client({ intents: [Intents.FLAGS.GUILDS, Intents.FLAGS.GUILD_MESSAGES] });

client.on('ready', () => {
  console.log(`Logged in as ${client.user.tag}!`);
});

client.on('message', message => {
  if (message.content === 'ping') {
    message.channel.send('pong');
  }
});

client.login('token');```
