# arch-playground-spring 

> "How can I die, when I have so much of the Universe left to explore?" - Stephen Hawking

Have fun hacking.

## Roadmap

* include font into service-worker

## Setup

> Use [IntelliJ](https://www.jetbrains.com/idea/download) for coding.

Simply open the cloned github folder and the gradle import wizard should pop up.

Install client dependencies:

    $ yarn install

## Production

Build client:

    $ yarn build

Build server:

    $ gradle build

Start server:

    $ java -jar build/libs/arch-playground-spring.jar

## Development

Start client watcher:

    $ yarn start

Start server:

    $ gradle bootRun [--debug-jvm]

## Testing

### Test client

    $ yarn test

### Test server

    $ gradle test

### Test e2e

#### Test e2e on selenium grid

    $ yarn test:e2e
    
#### Test e2e locally

    $ yarn webdriver:install
    $ yarn webdriver:start
    $ yarn test:e2e:local

## Dependency Update

Client dependencies:

    $ yarn dependency-update

Server dependencies:

    $ gradle dependencyUpdates -Drevision=release
