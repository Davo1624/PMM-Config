This config leverages the default kometa profiles with a few modifications as well as my own personal collections.

There are several files named `*.yml.back` which are now deprecated but I have kept for informational purposes.

These config files assume you are running the latest "nightly" branch.

I have now included a separate config-dv.yml file and associated builder file since kometa only allows one radarr instance per config. I run this config file daily on a cron job `docker exec kometa kometa.py -c /config/config-dv.yml -rl Movies -co -r` which will then populate the FEL/MEL plex collections with any files that have a FEL or MEL hdr layer.
