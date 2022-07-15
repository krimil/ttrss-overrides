# ttrss-overrides
Repo to store my TT-RSS override yaml and create nightly database backups using rclone to Google Drive

## Set up TT-RSS
```
git clone https://git.tt-rss.org/fox/ttrss-docker-compose.git ttrss-docker
```

## Clone this repo to ttrss-docker folder
```
git clone https://github.com/krimil/ttrss-overrides.git ttrss-overrides
```

```
cp ttrss-overrides/docker-compose.override.yml ttrss-docker/
```

Copy .env-dist to .env
Add entries from .env-overrides file to .env file
Populate values in .env file

Make directories
```
cd ~
mkdir -p tt-rss/app
mkdir -p tt-rss/backups
mkdir -p tt-rss/db
mkdir backups
mkdir rclone
```

Create rclone.conf file in ~/rclone


Fix requestIdleCallback error in Safari
```
curl https://raw.githubusercontent.com/pladaria/requestidlecallback-polyfill/master/index.js -o ~/tt-rss/app/tt-rss/themes.local/local-overrides.js
```
```
chmod 0644 ~/tt-rss/app/tt-rss/themes.local/local-overrides.js
```
