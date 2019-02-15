# DIPC-BOT
Telegram bot made for DIPC. This project is not finished and shouldn't be deployed as is. The Pytho bot is based on [Vzemtsov's ssh-connection-in-telegram project](https://github.com/vzemtsov/ssh-Connection-In-Telegram).

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Things you may need to install this project

```
Python 3.x
A web server (I used Apache2)
A telegram bot token
```

### Installing

Clone the repository to your web server root directory.

```
git clone 
```
Create a Telegram bot ([Official tutorial](https://core.telegram.org/bots#6-botfather)]) and make sure to write down your bot's token.  

Edit www/telegram-bot-py/config.py and add your parameters. 'botToken' refers to your bot's token, generated by BotFather.

Your bot should be ready to go. Run the next command from www/telegram-bot-py/ to run it.
```
python bot.py
```
You can now interact with it via Telegram. You should make sure your web server is properly set up to be able to access to it's full potential.

### Commands

* /on - login
* /off - logout
* /connect - Connect to a cluster
* /howto - User guide
* /information - Show information, about ssh-connection
* /aboutBot - Information about bot and author

The following commands are only allowed if you are connected to a cluster:
* /consumption - Check current consumption
* /queue - Show job queue
* /scratch - See used scratch space
* /dcrab - See dcrab report of a job

## Deployment

The bot is deployed by default. You only need to make your web server public so other users can access to the login page.

## Built With

* [Python](https://www.python.org/) - Programming language used to make bot logic
* [Apache2](https://httpd.apache.org/) - Web server used

## Contributing

This project is closed and doesn't accept contributions anymore. Nevertheless, you can always fork it and have fun developing more features!

## Authors

* **[Urko Lekuona](https://github.com/UrkoLekuona)**

See also the list of [contributors](https://github.com/UrkoLekuona/DIPC-BOT/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Acknowledgments

* [Vzemtsov](https://github.com/vzemtsov/)
