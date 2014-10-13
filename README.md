apiaryio
=============

Apiary.io CLI

[![Build Status](https://travis-ci.org/apiaryio/apiary-client.png?branch=master)](https://travis-ci.org/apiaryio/apiary-client)


## Install

**install gem** (required)
``` bash
gem install apiaryio
```

**setup APIARY.io credentials** (required for publish and fetch command only)

1. Retrieve APIKEY on `https://login.apiary.io/tokens`
2. Save it to your environment variables :

```bash
export APIARY_API_KEY=<your_token_retrieved_on_step_1>
```

## Description

Apiaryio gem provides a way to display your API documentation on your local
machine, either using static files or using a standalone web server...

## Usage

    $ apiary help

    Commands:
      apiary fetch --api-name=API_NAME    # Fetch apiary.apib from API_NAME.apiary.io
      apiary help [COMMAND]               # Describe available commands or one specific command
      apiary preview                      # Show API documentation in default browser
      apiary publish --api-name=API_NAME  # Publish apiary.apib on docs.API_NAME.apiary.io
      apiary version                      # Show version

    $ apiary help fetch
    
    Usage:
      apiary fetch --api-name=API_NAME

    Options:
      --api-name=API_NAME
      [--api-host=HOST]    # Specify apiary host
      [--output=FILE]      # Write apiary.apib into specified file

    Fetch apiary.apib from API_NAME.apiary.io    
    
    $ apiary help publish

    Usage:
      apiary publish --api-name=API_NAME

    Options:
      [--message=COMMIT_MESSAGE]  # Publish with custom commit message
      [--path=PATH]               # Specify path to blueprint file
                                  # Default: apiary.apib
      [--api-host=HOST]           # Specify apiary host
      --api-name=API_NAME

    Publish apiary.apib on docs.API_NAME.apiary.io
    
    $ apiary help preview

    Usage:
      apiary preview

    Options:
      [--browser=chrome|safari|firefox]  # Show API documentation in specified browser
                                         # Possible values: chrome, safari, firefox
      [--output=FILE]                    # Write generated HTML into specified file
      [--path=PATH]                      # Specify path to blueprint file
                                         # Default: apiary.apib
      [--api-host=HOST]                  # Specify apiary host
      [--server], [--no-server]          # Start standalone web server on port 8080
      [--port=PORT]                      # Set port for --server option

    Show API documentation in default browser

## Copyright

Copyright 2012-14 (c) Apiary Ltd.

## Contributors

- Jakub Nešetřil
- James Charles Russell [botanicus]
- Lukáš Linhart [Almad]
- Emili Parreño
- Peter Grilli [Tu1ly]
- Ladislav Prskavec
- Honza Javorek
- Matthew Rudy Jacobs
- Adam Kliment
- Jack Repenning
- Peter Strapp
- Pierre Merlin
- František Hába
- Benjamin Arthur Lupton

## License

Released under MIT license. See LICENSE file for further details.
