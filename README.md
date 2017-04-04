# Simple Test to use ActionCable


### Configuration
clone the repository:
```sh
$ git clone https://github.com/ralicata/rails51test.git
```

install Redis via Homebrew
```sh
$ brew update
$ brew install redis
```

install Yarn via Homebrew
```sh
$ brew install yarn
```

Add jQuery via Yarn
```sh
$ yarn add jquery
```

Launch servers in 2 different shells
```sh
$ redis-server
```
```sh
$ rails server
```

### Usage
Launch rails console in another shell
```sh
$ rails console
```
inside the console type:
```sh
Running via Spring preloader in process 20569
Loading development environment (Rails 5.1.0.rc1)
irb(main):001:0> ActionCable.server.broadcast 'web_notifications_channel', message: '<p>This is a message</p>'
```
