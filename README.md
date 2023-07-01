mtasic85.github.io
==================

mtasic85.github.io


## Prepare Env

```
$ gem install jekyll bundler
```

In `~/.bashrc` edit `PATH` env var:
```
...
PATH=$PATH:$HOME/.local/share/gem/ruby/3.0.0/bin
```


## Initially Create Blog

```
$ jekyll new --skip-bundle .
``` 


## Install gems
```
$ bundle install --path vendor/bundle
```


## Run Website
```
$ bundle exec jekyll serve
```
