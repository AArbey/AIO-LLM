# llm-server-aio
An all in one llm server configured from a docker compose file

This guide was made to be used on a debian server

## Prerequisites

### Nvidia drivers

These are commands i think worked for me, i currently didn't have time to try again a clean install of the nvidia drivers

```bash
apt update
apt install linux-headers-$(uname -r)
```

### Docker and Docker compose

```bash
# https://docs.docker.com/engine/install/debian/
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh ./get-docker.sh
```

## Installation process

Clone the repo :
```bash
git clone https://github.com/AArbey/llm-server-aio.git
cd llm-server-aio
```

Copy the .env.template and edit it with your own info.
```bash
cp .env.template .env
nano .env
```

Run with docker compose
```bash
docker compose up -d
```

