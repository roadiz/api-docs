# Roadiz API documentation generator
Built on [Sami](https://github.com/FriendsOfPHP/sami), the API Documentation Generator.

## Install
Make sure that `sami.phar` command is available.

Once you’ve cloned this project:

```bash
curl -O http://get.sensiolabs.org/sami.phar;

# Make sure that our custom theme is up to date
git submodule init;
git submodule update;

# Copy sample config
cp config.php.sample config.php;

# Edit config.php to set Roadiz project path
# Roadiz vendors should be present (composer install)
nano config.php

# Launch Sami generation
sami.phar update config.php

# Update
rsync -azc --delete -e ssh ./build/master/ xxxxxxxxx@api.roadiz.io:~/public_html/
```