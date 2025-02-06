# About this fork of a project
Bypass check if user has a real Microsoft account linked with the launcher<br>

⚠️ This is for entertainment purposes only ⚠️

# Before Installation
If you have some accounts saved then executing this script will remove them! Don't forget to backup your "accounts.json" file if needed!

# How to use
- Install Prism Launcher
- Go through the quick setup
- CLOSE THE LAUNCHER
- Execute the command for the appropriate bypass (see [below](#usage-for-installer))
- Create an offline account
- Set the newly created account as the default
- Enjoy!

# What not to do
Don't delete the "No Profile" account, that will break the bypass!

# How does this work?
This launcher use a file called "accounts.json" which stores information about user's accounts. It also indicates whether a user owns Minecraft. This functionality allows players to play Minecraft even if they are offline, such as when playing on a Steam Deck in the middle of a forest. This feature can be exploited to gain access to the launcher and Minecraft's assets.

# Custom Skins?
For that luxury you can use Ely.by skin system on the [ElyPrismLauncher](https://github.com/Octol1ttle/ElyPrismLauncher)

# Usage for Installer
Download the latest version of Prism Launcher from https://prismlauncher.org/, install it, go through the quick setup, close the launcher, then execute this command in the terminal:
### Windows CMD:
```
echo {
    "accounts": [
        {
            "entitlement": {
                "canPlayMinecraft": true,
                "ownsMinecraft": true
            },
            "msa-client-id": "",
            "type": "MSA"
        },
        {
            "active": true,
            "entitlement": {
                "canPlayMinecraft": true,
                "ownsMinecraft": true
            },
            "profile": {
                "capes": [
                ],
                "id": "0c79d88a112537a0a302f01afa6bc94a",
                "name": "YOUR-NICKNAME",
                "skin": {
                    "id": "",
                    "url": "",
                    "variant": ""
                }
            },
            "type": "Offline",
            "ygg": {
                "extra": {
                    "clientToken": "8be89b1112474b5fb8f061699ff41bda",
                    "userName": "YOUR-NICKNAME"
                },
                "iat": 1738858981,
                "token": "0"
            }
        }
    ],
    "formatVersion": 3
} > %appdata%/PrismLauncher/accounts.json
```
### Linux Shell:
```
echo '{
    "accounts": [
        {
            "entitlement": {
                "canPlayMinecraft": true,
                "ownsMinecraft": true
            },
            "msa-client-id": "",
            "type": "MSA"
        },
        {
            "active": true,
            "entitlement": {
                "canPlayMinecraft": true,
                "ownsMinecraft": true
            },
            "profile": {
                "capes": [
                ],
                "id": "0c79d88a112537a0a302f01afa6bc94a",
                "name": "YOUR-NICKNAME",
                "skin": {
                    "id": "",
                    "url": "",
                    "variant": ""
                }
            },
            "type": "Offline",
            "ygg": {
                "extra": {
                    "clientToken": "8be89b1112474b5fb8f061699ff41bda",
                    "userName": "YOUR-NICKNAME"
                },
                "iat": 1738858981,
                "token": "0"
            }
        }
    ],
    "formatVersion": 3
}' > ~/.local/share/PrismLauncher/accounts.json
```
### Linux Shell (flatpak):
```
echo '{
    "accounts": [
        {
            "entitlement": {
                "canPlayMinecraft": true,
                "ownsMinecraft": true
            },
            "msa-client-id": "",
            "type": "MSA"
        },
        {
            "active": true,
            "entitlement": {
                "canPlayMinecraft": true,
                "ownsMinecraft": true
            },
            "profile": {
                "capes": [
                ],
                "id": "0c79d88a112537a0a302f01afa6bc94a",
                "name": "YOUR-NICKNAME",
                "skin": {
                    "id": "",
                    "url": "",
                    "variant": ""
                }
            },
            "type": "Offline",
            "ygg": {
                "extra": {
                    "clientToken": "8be89b1112474b5fb8f061699ff41bda",
                    "userName": "YOUR-NICKNAME"
                },
                "iat": 1738858981,
                "token": "0"
            }
        }
    ],
    "formatVersion": 3
}' > ~/.var/app/org.prismlauncher.PrismLauncher/data/PrismLauncher/accounts.json
```
### macOS
```
echo '{
    "accounts": [
        {
            "entitlement": {
                "canPlayMinecraft": true,
                "ownsMinecraft": true
            },
            "msa-client-id": "",
            "type": "MSA"
        },
        {
            "active": true,
            "entitlement": {
                "canPlayMinecraft": true,
                "ownsMinecraft": true
            },
            "profile": {
                "capes": [
                ],
                "id": "0c79d88a112537a0a302f01afa6bc94a",
                "name": "YOUR-NICKNAME",
                "skin": {
                    "id": "",
                    "url": "",
                    "variant": ""
                }
            },
            "type": "Offline",
            "ygg": {
                "extra": {
                    "clientToken": "8be89b1112474b5fb8f061699ff41bda",
                    "userName": "YOUR-NICKNAME"
                },
                "iat": 1738858981,
                "token": "0"
            }
        }
    ],
    "formatVersion": 3
}' > ~/Library/Application\ Support/PrismLauncher/accounts.json
```

# Usage for Portable version
Download the portable version of [Prism Launcher](https://prismlauncher.org/), run it, go through the quick setup, close the launcher, then execute this command in the terminal:
### Windows Portable (cd to installation path) CMD:
```
echo {
    "accounts": [
        {
            "entitlement": {
                "canPlayMinecraft": true,
                "ownsMinecraft": true
            },
            "msa-client-id": "",
            "type": "MSA"
        },
        {
            "active": true,
            "entitlement": {
                "canPlayMinecraft": true,
                "ownsMinecraft": true
            },
            "profile": {
                "capes": [
                ],
                "id": "0c79d88a112537a0a302f01afa6bc94a",
                "name": "YOUR-NICKNAME",
                "skin": {
                    "id": "",
                    "url": "",
                    "variant": ""
                }
            },
            "type": "Offline",
            "ygg": {
                "extra": {
                    "clientToken": "8be89b1112474b5fb8f061699ff41bda",
                    "userName": "YOUR-NICKNAME"
                },
                "iat": 1738858981,
                "token": "0"
            }
        }
    ],
    "formatVersion": 3
} > accounts.json
```
### Linux Portable (cd to installation path) Shell:
```
echo '{
    "accounts": [
        {
            "entitlement": {
                "canPlayMinecraft": true,
                "ownsMinecraft": true
            },
            "msa-client-id": "",
            "type": "MSA"
        },
        {
            "active": true,
            "entitlement": {
                "canPlayMinecraft": true,
                "ownsMinecraft": true
            },
            "profile": {
                "capes": [
                ],
                "id": "0c79d88a112537a0a302f01afa6bc94a",
                "name": "YOUR-NICKNAME",
                "skin": {
                    "id": "",
                    "url": "",
                    "variant": ""
                }
            },
            "type": "Offline",
            "ygg": {
                "extra": {
                    "clientToken": "8be89b1112474b5fb8f061699ff41bda",
                    "userName": "YOUR-NICKNAME"
                },
                "iat": 1738858981,
                "token": "0"
            }
        }
    ],
    "formatVersion": 3
}' > accounts.json
```

# Manual Installation
There is a file in the repository called [accounts.json](accounts.json) and you need to download it to this path:
### Installer
* Windows: `%appdata%/PrismLauncher/`
* Linux: `~/.local/share/PrismLauncher/`
* Linux (flatpak): `~/.var/app/org.prismlauncher.PrismLauncher/data/PrismLauncher/`
* macOS: `~/Library/Application\ Support/PrismLauncher/`

### Portable
In the root directory of the launcher
