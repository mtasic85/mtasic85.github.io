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
PATH=$PATH:/home/mtasic-arch/.gem/ruby/2.7.0/bin
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
