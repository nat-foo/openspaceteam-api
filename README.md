# OpenSpaceTeam API
OpenSpaceTeam is an open source implementation of a 
[Spaceteam](http://spaceteam.ca/)-like game, playable through the 
browser. This is a fork from [OpenSpaceTeam's](https://github.com/openspaceteam) [backend](https://github.com/openspaceteam/backend), which referenced a separate [frontend repo](https://github.com/openspaceteam/frontend). As the original author is no longer active, I've forked both and updated them to work in 2022. As the base engine is quite flexible, I may push this in a new direction if I have the time.

## Changelog
1. [02/06/22] Updated packages and fixed related bugs.

## Requirements
- Python 3.6 (doesn't work in <= 3.5 nor 2)
- An SSL certificate (not required but highly recommended)

## Installing
```bash
$ git clone https://github.com/nat-foo/openspaceteam-api.git
$ cd openspaceteam-api
$ virtualenv -p $(which python3.6) .pyenv
$ source .venv/bin/activate
(.pyenv)$ pip install -r requirements.txt

# SSL is optional, but recommended
(.pyenv)$ mv certs/spaceteam.crt cert.crt
(.pyenv)$ mv certs/spaceteam.key key.key


(.pyenv)$ cp settings.sample.ini settings.ini
(.pyenv)$ nano settings.ini
...
(.pyenv)$ python3 spaceteam.py

  __  ___  __   ______ _____ ___  __  __ __
/' _/| _,\/  \ / _/ __|_   _| __|/  \|  V  |
`._`.| v_/ /\ | \_| _|  | | | _|| /\ | \_/ |
|___/|_| |_||_|\__/___| |_| |___|_||_|_| |_|


INFO:root:Using SSL
======== Running on http://0.0.0.0:4433 ========
(Press CTRL+C to quit)
```

## Configuring
The easiest configuration is letting the backend listen on all interfaces (0.0.0.0) and using a SSL certificate by
[Let's Encrypt](https://letsencrypt.org/).
Put the certificate (rename it to `cert.crt`) and the key file (rename it to `key.key`) in backend's folder. You can
specify a different path as well in `settings.ini`.

## License
This project is licensed under the GNU AGPL 3 License. See the "LICENSE" file for more information.

