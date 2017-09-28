# Intercom Export

Export data from Intercom. Currently supports only conversations.

## Installation

### Dependencies

- `docker`: check installation instructions [in Docker official website](https://www.docker.com/).
- `mruby-cli`: actually don't need to install, Docker will handle this dependency. Anyway, see [mruby-cli](https://github.com/hone/mruby-cli) for more details. 

After installing and configuring `docker` and `docker-compose`, you'll be able to install Intercom Export, `mruby-cli` and other needed dependencies with a single Docker command. In order to do that, just clone/download this project into your PC and run the following command from your Terminal (run inside this project folder):

```
docker-compose run compile
```

And you're done!

## Usage

For now, you can only export all the conversations and prints them on stdout

```
./mruby/build/host/bin/intercom-export -t <API KEY>:<API SECRET> -r conversations
```

## Contributing

1. Fork it ( https://github.com/toch/intercom-export/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
