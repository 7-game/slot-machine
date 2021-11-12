Slot Machine buildpack
=======================

This is an example [Heroku Slot Machine](http://devcenter.heroku.com/articles/buildpacks).

Usage
-----

Example usage:

    $ ls
    slot.js

    $ heroku create --stack cedar --buildpack https://github.com/7-game/slot-machine.git

    $ git push heroku master
    ...
    -----> Heroku receiving push
    -----> Fetching custom buildpack
    -----> SlotMachine app detected
    -----> Found a slot.js

The buildpack will detect that your app has a `slot.js` in the root. If this file has contents, it will be copied to `slot-run.js`.

Add tags
