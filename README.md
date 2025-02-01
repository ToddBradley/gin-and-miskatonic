# Gin and Miskatonic

This GitHub project is a website for a Call of Cthulhu RPG campaign. The players are in Colorado in the year 2024. The characters are in New England in the 1920s.

## Building

Unless something is messed up, there are GitHub Actions that automatically build and deploy this site whenever a new commit is pushed. Look for the site to be hosted at https://toddbradley.github.io/gin-and-miskatonic.

## Todd's Notes

Here's what to do to start over and rebuild the development environment for this site.

https://jekyllrb.com/docs/installation/macos/


### Install Ruby and Jekyll

```
brew install chruby ruby-install
ruby-install ruby 3.4.1
```

Configure shell to use this ruby:

```
echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
echo "chruby ruby-3.4.1" >> ~/.zshrc # run 'chruby' to see actual version
```

Restart the shell, and make sure ruby is using 3.4.1.

Install Jekyll.

```
gem install jekyll
```

### Now get started

Delete the Gemfile and create a new one

```
gem install jekyll bundler
bundle init
```

Edit Gemfile to add this: `gem "jekyll"`

> You can now prefix all jekyll commands listed in this tutorial with bundle exec to make sure you use the jekyll version defined in your Gemfile.



Ultimate goal:

bundle exec jekyll serve
