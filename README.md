# Urban Platform Cameroon

## Requirements

- [**Docker**](https://docs.docker.com/desktop/) with compose plugin

*If you are using **Windows** :*
- [**WSL 2**](https://docs.docker.com/desktop/wsl/#turn-on-docker-desktop-wsl-2)
- [**VSCode WSL extension**](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-wsl)

## Getting started

To setup your local env project (Only the first time)

``` bash
# Clone your project
# ⚠️ On Windows make sure you are cloning it from your WSL environnement
git clone git@github.com:GeOsmFamily/IDG_Douala.git idg && cd idg

# Build and pull your docker images 🐋 & setup your hosts local domains
make init

# make a copy of .env file and name it .env.local
cp .env .env.local

# run docker container
docker compose up -d --build

# fill the database with mock data
make rerun-database

# update the hosts file system with adding idg.local domain.
C:\Windows\System32\drivers\etc\hots

# then open your browser and enter the domain to access your website
https://idg.local/
```

Enjoy ! 🚀