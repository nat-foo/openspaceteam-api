# OpenSpaceTeam API
OpenSpaceTeam is an open source implementation of a 
[Spaceteam](http://spaceteam.ca/)-like game, playable through the 
browser. This is a fork from [OpenSpaceTeam's](https://github.com/openspaceteam) [backend](https://github.com/openspaceteam/backend), which referenced a separate [frontend repo](https://github.com/openspaceteam/frontend). As the original author is no longer active, I've forked both and updated them to work in 2022. As the base engine is quite flexible, I may push this in a new direction if I have the time.

## Changelog
1. [02/06/22] Updated packages and fixed related bugs.

## Requirements
- Python 3.6 (doesn't work in <= 3.5 nor 2. Check with `python --version`. May have to use `python3`.)
- PIP (check with `pip --version`)
- VirtualEnv (for Mac setup see [here](https://sourabhbajaj.com/mac-setup/Python/virtualenv.html))

## Installing
```bash
$ git clone https://github.com/nat-foo/openspaceteam-api.git
$ cd openspaceteam-api
$ virtualenv -p $(which python3.6) .venv
$ source .venv/bin/activate
(.venv)$ pip install -r requirements.txt
(.venv)$ python3 spaceteam.py

  __  ___  __   ______ _____ ___  __  __ __
/' _/| _,\/  \ / _/ __|_   _| __|/  \|  V  |
`._`.| v_/ /\ | \_| _|  | | | _|| /\ | \_/ |
|___/|_| |_||_|\__/___| |_| |___|_||_|_| |_|


INFO:root:Using SSL
======== Running on http://0.0.0.0:4433 ========
(Press CTRL+C to quit)
```

Let that run in the background and now connect with the client.

## License
This project is licensed under the GNU AGPL 3 License. See the "LICENSE" file for more information.

