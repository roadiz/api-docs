# Roadiz API documentation generator
Built on [Sami](https://github.com/FriendsOfPHP/sami), the API Documentation Generator.

## Install
Make sure that `sami` command is available.

Once you’ve cloned this project:

```
git submodule init;
git submodule update;

# Copy sample config
cp config.php.sample config.php;
# Edit config.php to set Roadiz project path
nano config.php
# Launch Sami generation
sami update config.php

# Update
rsync -azc --delete -e ssh ./build/master/ xxxxxxxxx@api.roadiz.io:~/public_html/
```