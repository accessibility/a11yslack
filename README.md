# A11y Slack

A dedicated accessibility space to ask questions, help other people figure stuff out or chat about accessibility in general.

We want this to be a fun, pleasant, and harassment-free experience for everyone, regardless of gender, gender identity and expression, sexual orientation, disability, physical appearance, body size, race, or religion. We do not tolerate harassment or intimidation of participants in any form. Participants asked to stop any harassing behavior are expected to comply immediately.

This GitHub Pages site is powered by [Jekyll](https://jekyllrb.com/) and the [Cayman](https://github.com/pages-themes/cayman) GitHub Pages theme. You don't need to install anything locally to modify existing pages or add new ones, but follow the instructions below if you want to make more significant changes to the structure of the site.

## Building locally

First, ensure that you have a recent version of Ruby installed locally.

On a Mac, you can install [rbenv](https://github.com/rbenv/rbenv) using [Homebrew](https://brew.sh/) and install a compatible version of Ruby 3.x to run within this directory. *Version 4.x of Ruby is not compatible with GitHub Pages, which is still running on Jekyll 3.*

```
brew install rbenv

rbenv init # follow the instructions to add rbenv to your shell environment

rbenv install 3.4.12 # install the correct Ruby version for this repo on your machine

cd path/to/your/repo
rbenv local  # run this command to set/confirm the Ruby version for just this project
```

If any of these commands don't work as they should, you may need to quit and re-open your terminal app/tab before trying again.

Once you have a sensible Ruby environment up and running, run these two commands to install dependencies:
```
gem install bundler
bundle install
```

Finally, run this command to generate the static site and serve it locally at [localhost:4000](http://localhost:4000/):
```
bundle exec jekyll serve
```

As you edit files and save them, the static site will automatically rebuild. You will need to refresh the page to see your changes. Changes to `_config.yml` won't always be automatically reflected - you might need to stop the Jekyll serve process (Ctrl/Cmd + C) and restart it before you can see them.
