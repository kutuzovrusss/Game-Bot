# Game-Bot

This Discord bot takes in a Steam game's name and returns its link on the Steam Store based on Valve's search suggest feature.

[![Discord Bots](https://discordbots.org/api/widget/397546577314578433.svg)](https://discordbots.org/bot/397546577314578433)

## Dependencies

`discord.py`, `lxml`, `aiohttp`, `sqlitedict`, `psutil`, `dblpy`:
```
python3 -m pip install --user discord.py lxml aiohttp sqlitedict psutil dblpy
```

Set the environment variable `GAME_BOT_TOKEN` as your token, eg.

```
export GAME_BOT_TOKEN=foobar
python3 game_bot.py
```

If you have `HISTCONTROL` set to `ignoreboth` or `ignorespace` in bash,
prepend a space before any command containing your token to prevent it from
showing up in your history.

**Make sure you are running Python 3.4.2+!**

## To do:
* Consider alternative strategy when game isn't on steam store rather than hard-coding (maybe IGDB) 

* <del>Consider mapping game exceptions (like for CSGO and TF2) in a dictionary to replace the else if statements</del>

* <del>When a game isn't found, react to the user's message with a crying emoji.</del>

* <del>Add server counter for DiscordBots.org</del>

* <del>Change "Try again with more characters or a different game!" to "Try again with less characters or a different game!"</del>

* <del>Remove "Looking for x" string output, and set up "Game not found" instead.</del>
