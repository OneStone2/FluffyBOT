
# Cookie Run Kingdom: Guild Battle BOT


[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
## Installation

Install Dependencies through `pip` via command line

```bash
  pip install -r requirements.txt
```
    
## Features 📙

- Allows users to attack bosses 'stored' in Discord channels
- Serializes all data to `json` and can export all data in sorted `csv` file
- Admins can fix different user errors with `admin` commands
- Integrated with descriptive slash commands
## Documentation 📄
Click here to read the 
[Documentation](https://onioncult.com/documentation/standalone.html) on how to use the bot commands and read their usages.


## Deployment 🚀

### Commands you need to change to an 'admin' role in App Integration settings:

```bash
  admin_hit
  admin_kill
  admin_revive
  create_boss
  delete_boss
  insert_boss
  load_json
  send_backup_csv
  send_csv
```

### Files you need to change to get the project deployed:

```bash
  bot.py
  tkn.txt
```
Note that `tkn.txt` is *not* included in the repo -- you will need to create this yourself.
Put the token of your bot in this file on the first line.

In `bot.py` you will need to change:

- `guild_ids` -> Guilds/Servers that can use the bot
- `valid_channels` (optional) -> Names of channels bosses can be created in
- `guilds` -> Change to any sister guilds (not servers) that can use the bot
- `ping_roles` -> IDs of roles to be pinged when bosses are killed
- `sweeper_roles` and `sweeper_requirements` -> IDs of roles and requirements for each guild
- `split_threshold` -> How many hits users are 'allowed' per boss level to encourage splitting

## Lessons Learned 👨‍🏫

This project has taught me a LOT. From how the Discord API works, to managing every
single edge case I could think of: I see this as the most valuable project I've taken on.

I feel much more confident when reading documentation and formulating ways to ask the right
questions in order to progress through hurdles.

I've also learned a lot about how async functions work, and how API calls are handled.
Switching from using normal commands to app commands (slash commands) has been extremely
useful with regards to learning how a lot of Discord functions work internally.

Additionally, I've learned a lot about different packages that Python has to offer.
For example, serializing and deserializing data to json via the attrs/cattrs packages has been an
invaluable experience! I have almost 10 dependencies in this project, so learning about
different ways to accomplish my goals through these packages has been a great experience.

Finally, I feel like this project has been a great project to refine my Python and overall programming
skills! I've made some projects in Python before, but this one was on a whole new level. In general,
I've had to branch out and learn multiple new programming concepts on my own through this
project. From data serialization, to asynchronous functions, to some DSA, to blocking code:
this project tested me in every way.

## Acknowledgements ♥

 - [discord.py Discord Server](discord.gg/dpy)
 - [Alex Zades -- helped with cattrs](https://github.com/AlexZades)
 - [OnionCult Discord! -- there wouldn't be a bot without them to use it!](https://discord.com/invite/onioncult)
 - [VanLyden/Lama](https://sites.google.com/view/lama-alnatour/about) -- all the art for the bot was kindly done by her!
