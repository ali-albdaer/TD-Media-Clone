# TelegramDiscordClone

TelegramDiscordClone is a Python script that utilizes discord.py and telethon libraries to clone messages, including media, from a Telegram group to a specified Discord channel. It achieves this by logging into a Telegram user account, temporarily downloading the messages in chronological order, and then sending them to Discord using a webhook.

## Key Features

- Clones messages and media files by simply
- Has configurable parameters such as `IGNORE_VIDEO_FILES`, `CLONE_MEDIA_ONLY`, `SHOW_USER_INFO` etc. (See [example](config_example.py))
- Temporarily stores the last porcessed message and media file, contiues from where it left if the program crashes / halts.
- Uses [dummyimage](https://dummyimage.com) to genearte dynamic profile pictures for people without a pfp. (Thanks to [Russell Heimlich](https://dummyimage.com/#about) for providing this free tool)


## Installation

1. Clone the repository: `git clone https://github.com/ali-albdaer/TelegramDiscordClone.git`
2. Install the required dependencies: `pip install -r requirements.txt`

## Configuration

1. Create a Discord channel and a webhook for that channel then obtain the link.
2. Create a new Telegram app and obtain the API ID and API hash. (visit https://my.telegram.org)
3. Create a `config.py` file in the root directory, put the obtained credentials and adjust the other parameters as needed. (See [example](config_example.py))

## Usage

1. Run the `main.py` script: `python main.py`
2. When used for the first time, the script will prompt you to log in to your Telegram account.
3. Once logged in, it will start cloning the messages from the Telegram group.
4. The cloned messages will be sent to the specified Discord channel via the webhook.

## DISCLAIMER

This script is designed to back up data from Telegram to Discord in a fun and convenient way. 
It was created with the intention of providing a useful tool for personal use and small communities.

Please use this script responsibly and in accordance with the terms of service of both Telegram and Discord.
Avoid using it for any malicious or unauthorized activities. I'm not responsible for any misuse
or potential breaches of privacy that may arise from improper use of this script.

Remember to respect the privacy and permissions of others when handling and sharing data.

Happy cloning!

## Contributing

You are more than welcome to contribute to this project. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
