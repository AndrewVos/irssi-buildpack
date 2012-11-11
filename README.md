irssi-buildpack
===============

What?
-----
Want IRSSI running on a free Heroku instance? That's what this is.

Want!
-----

    mkdir irssi
    cd irssi
    heroku create <SOMETHING_UNIQUE>-irssi --buildpack https://github.com/AndrewVos/irssi-buildpack
    mkdir .irssi
    touch .irssi/config
    git init
    git add .
    git commit -m "add irssi config"
    git push heroku master

Now you can ssh into the box (this probably needs work)

    heroku run bash
And run irssi

    ./vendor/irssi/bin/irssi
