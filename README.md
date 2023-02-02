# Docker Container for Leek<br>[![GitHub Actions][actions-img]][actions-url] [![Patreon][patreon-img]][patreon-url] [![PayPal][paypal-img]][paypal-url] [![Discord][discord-img]][discord-url]

> WARNING: Please note that Leek is an experimental work in progress project, and as such, the API might change unexpectedly at any time.

This is a simple way to use a Docker container to run Leek and all of it's data with a MariaDB.

## Installation

You will first need to clone the entire repo and modify it to fit your needs. You can do so by running the following command(s):

```
git clone https://github.com/LeekByLemon/Leek.git leek
cd leek
```

## Usage

Just like the Leek package, [you need to connfigure it using a .env file](https://github.com/LeekByLemon/Leek#usage). The only difference is that you also need to add a root password for the MariaDB instance. The right way to do this is by setting the value of MARIADB_ROOT_PASSWORD, but you can also [use any of the other root password options allowed by MariaDB](https://github.com/docker-library/docs/tree/master/mariadb#environment-variables).

If you want to add more cogs from other places, you can add their repos in `requirements.txt` and they will be installed when you build the Docker image.

After configuring Leek, you just start it with Docker Compose by using `docker compose up -d`. Everything will start automatically with the provided options.

[actions-img]: https://img.shields.io/github/actions/workflow/status/LeekByLemon/LeekDocker/main.yml?branch=master&label=actions
[actions-url]: https://github.com/LeekByLemon/Leek/actions
[patreon-img]: https://img.shields.io/badge/support-patreon-FF424D.svg
[patreon-url]: https://www.patreon.com/lemonchan
[paypal-img]: https://img.shields.io/badge/support-paypal-0079C1.svg
[paypal-url]: https://paypal.me/justalemon
[discord-img]: https://img.shields.io/badge/discord-join-7289DA.svg
[discord-url]: https://discord.gg/Cf6sspj
