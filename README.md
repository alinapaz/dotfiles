# dotfiles
Workstation setup and configuration

## Installing packages with Homebrew

Most development tools can and should be installed via [Homebrew](http://brew.sh/), for example:

- chruby (for changing Ruby versions): `brew install chruby`
- ruby-install (for installing new Ruby versions): `brew install ruby-install`
- Nodejs: `brew install node`

To update Homebrew itself `brew update`.

## Installing Ruby

Use `chruby` (for changing the version of Ruby used for different projects) and `ruby-install` (for installing new/different versions of ruby); don't use `rvm`. These can be installed via Homebrew (e.g. `brew install chruby ruby-install`).

- To list the availlable/installed versions of Ruby: `chruby` 
- To install the latest version of Ruby: `ruby-install ruby-2.3.0`
- Then to change to that version of Ruby `chruby 2.3.0`
- To verify the version of Ruby being used: `ruby -v`

# Installing Ruby Bundler and Ruby Gems

Bundler manages gems via a Gemfile. Confusingly, the gem is called `bundler`, but the commandline command is `bundle`

- To install bundler, run `gem install bundler` (this is the only gem you should ever install using `gem install`; always install all other gems using a Gemfile and the `bundle` command)
- To install gems using a Gemfile, use `bundle install`
