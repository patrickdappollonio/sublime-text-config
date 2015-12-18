# Sublime Text 3 Config Syncing

This repository holds my personal preferences of Sublime Text 3 to be shared in different computers by using simple Git commands. Essentially, it's a basic installation of [Package Control](https://packagecontrol.io/) plus the Sublime Settings per se.

The preference files are:

* [Sublime Text 3 Preference File](Preferences.sublime-settings)
* [Package Control Preference File](Package Control.sublime-settings)

There are also a few snippets useful for my daily work, such as:

* [A Goji Handler](GojiHandler.sublime-snippet) to be used in any project that uses [the great Goji library](http://goji.io/).
* [A basic, raw HTTP handler](HttpHandler.sublime-snippet) and [a raw HTTP middleware](HttpMiddleware.sublime-snippet) to be used with the `net/http` package.

### How can I do this on my own

Basically you can commit your config files to a Git repository of your preference. To know where that folder resides on your Hard Drive, go to your Sublime Text 3 Screen and click on `Preferences` then `Browse packages...`. From there, a File Manager window should open with the given path. 

There are a few files you might want to not include in the resulting repository such as cache files, or files that changes a lot overtime, such as:

* `Package Control.last-run`
* `Package Control.ca-list`
* `Package Control.ca-bundle`
* `Package Control.system-ca-bundle`
* `Package Control.cache/`
* `Package Control.ca-certs/`

So you might want to add those in your [gitignore file](.gitignore) and all other files who might give you trouble because they're updated too often or there's no winning by adding them to a source control.

There's also an alternative using Dropbox, if you have a few kilobytes left to spare. To go that way, please refer to the [Package Control Website](https://packagecontrol.io/docs/syncing) where you can read how to do it properly.
