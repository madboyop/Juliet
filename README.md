![Juliet](https://telegra.ph/file/929a3cffe8935f0a445e6.jpg)

# Juliet

[![Updates channel!](https://img.shields.io/badge/Join%20Channel-!-red)](https://telegram.me/Romeo_JulietBot_Support)



Can be found on telegram as [Juliet](https://telegram.me/Juliet2Bot).

The Support group can be reached out to at [Romeo & Juliet Bot Support](https://telegram.me/Romeo_JulietBotSupport), where you can ask for help about [Juliet](https://telegram.me/Juliet2Bot), discover/request new features, report bugs, and stay in the loop whenever a new update is available. 

## How to setup/deploy.

### Read these notes carefully before proceeding 
 - Edit any mentions of @OnePunchSupport to your own support chat
 - Your code must be open source and a link to your fork's repository must be there in the start reply of the bot [See this](https://github.com/madboyop/Juliet/blob/8c4c49b61c00d2618f620c813cc84ffdc0d2e38b/SaitamaRobot/__main__.py#L10)
 - Lastly, if you are found to run this repo without the code being open sourced or the repository link not mentioned in the bot, we will push a gban for you in our network because of being in violation of the license, you are free to be a dick and not respect the open source code (we do not mind) but we will not be having you around our chats
 - This repo does not come with technical support, so DO NOT come to us asking help about deploy/console errors

<details>
  <summary>Steps to deploy on Heroku !! </summary>

```
Fill in all the details, Deploy!
Now go to https://dashboard.heroku.com/apps/(app-name)/resources ( Replace (app-name) with your app name )
REMEMBER: Turn on worker dyno (Don't worry It's free :D) & Webhook
Now send the bot /start, If it doesn't respond go to https://dashboard.heroku.com/apps/(app-name)/settings and remove webhook and port.
```

  [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/madboyop/Juliet.git)

</details>  
<details>
  <summary>Steps to self Host!! </summary>

  ## Setting up the bot (Read this before trying to use!):
Please make sure to use python3.6, as I cannot guarantee everything will work as expected on older Python versions!
This is because markdown parsing is done by iterating through a dict, which is ordered by default in 3.6.

  ### Configuration

There are two possible ways of configuring your bot: a config.py file, or ENV variables.

The preferred version is to use a `config.py` file, as it makes it easier to see all your settings grouped together.
This file should be placed in your `SaitamaRobot` folder, alongside the `__main__.py` file. 
This is where your bot token will be loaded from, as well as your database URI (if you're using a database), and most of
your other settings.

It is recommended to import sample_config and extend the Config class, as this will ensure your config contains all
defaults set in the sample_config, hence making it easier to upgrade.

An example `config.py` file could be:
```
from SaitamaRobot.sample_config import Config

class Development(Config):
    OWNER_ID = 1078841825  # your telegram ID
    OWNER_USERNAME = "Warning_MadBoy_is_Here"  # your telegram username
    API_KEY = "your bot api key"  # your api key, as provided by the @botfather
    SQLALCHEMY_DATABASE_URI = 'postgresql://username:password@localhost:5432/database'  # sample db credentials
    JOIN_LOGGER = '-1234567890' # some group chat that your bot is a member of
    USE_JOIN_LOGGER = True
    DRAGONS = [1107922726]  # List of id's for users which have sudo access to the bot.
    LOAD = []
    NO_LOAD = ['translation']
```

If you can't have a config.py file (EG on Heroku), it is also possible to use environment variables.
So just go and read the config sample file. 


## How to setup on Heroku 
For starters click on this button 

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/madboyop/Juliet.git) 


## Credits
The bot is based on the original work done by <b>[PaulSonOfLars](https://github.com/PaulSonOfLars)</b>
All original credits go to Paul and his dedication, Without his efforts, this fork would not have been possible!

<b>Fork Developer --></b> <b><i>[MADBOY](https://github.com/madboyop)</i></b>
or <b><i>[MADBOY](https://telegram.me/Warning_MadBoy_is_Here)</i></b>

Also, missing proper credit for blacklistusers taken from TheRealPhoenixBot (will add it later, this note says unless it is done)

Any other authorship/credits can be seen through the commits.

Should any be missing kindly let us know at <b>[Romeo & Juliet Bot Support](https://telegram.me/Romeo_JulietBotSupport)</b> or simply submit a pull request on the readme.
