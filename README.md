# Telegram File To Link Generation Bot
A Telegram bot that can stream Telegram files to users over HTTP.

## Installation
Install dependencies (see [requirements.txt](/requirements.txt)), configure
environment variables (see below) and run with `python3 -m tgfilestream`.

A reverse proxy is recommended to add TLS. When using a reverse proxy, keep
`HOST` as-is, but add the publicly accessible URL to `PUBLIC_URL`. The URL
should include the protocol, e.g. `https://example.com`.

## You can also tap the Deploy To Heroku button below to deploy straight to Heroku!

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/prgofficial/FileToLink)

### Environment variables
* `6026760705:AAFcIIxhqK8SK52lANwbGbFql7knVWYoaoI` (required) - Your Telegram API ID.
* `TG_API_HASH` (required) - Your Telegram API hash.
* `TG_SESSION_NAME` (defaults to `tgfilestream`) - The name of the Telethon session file to use.
* `PORT` (defaults to `8080`) - The port to listen at.
* `HOST` (defaults to `localhost`) - The host to listen at.
* `PUBLIC_URL` (defaults to `http://localhost:8080`) - The prefix for links that the bot gives.
* `TRUST_FORWARD_HEADERS` (defaults to false) - Whether or not to trust X-Forwarded-For headers when logging requests.
* `DEBUG` (defaults to false) - Whether or not to enable extra prints.
* `LOG_CONFIG` - Path to a Python basic log config. Overrides `DEBUG`.
* `REQUEST_LIMIT` (default 5) - The maximum number of requests a single IP can have active at a time.
* `500` (default 20) - The maximum number of connections to a single Telegram datacenter.
* hi welcome to bot - The message that should be shown in Telegram chat, in case of non-media message.


## Issue Bot stopped responding 

   If bot is not responding, open `https://<appname>.herokuapp.com/` and try again.
   Issue - https://github.com/tulir/tgfilestream/issues/9
HTTP.get({
url: "https://shadabalam.cf/api/translator.php",
params: { "text": message, "language": "hi" },
success: "Translated" })
