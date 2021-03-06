# Fobit Game Platform

## Intro
In this game you have 32 yes/no decisions to take. You can think a lot and won the game.

Or you can try 4 billion times (2^³²) and won the game as well.

It is still in Alpha version so many things are not working.

## How to play online

* Access http://fobit.terahorse.com

## How to play anywhere using docker
* Install [Docker](https://docs.docker.com/install)
* Run `$ sudo docker run -d -p 80:5000 --name fobit terahorse/fobit`
* Access http://localhost

## Docker Images

Each release is launched at our [Docker Hub page](https://hub.docker.com/r/terahorse/fobit/tags/).
You can check also our releases notes in the CHANGELOG.md file.

## Rest API
| Call | Method | Description | Example |
| --- | --- | --- | --- |
| **/api/version** | GET | Gets current version | */api/version* |
| **/api/battle/{cardsCode}** | GET | Starts a new battle | */api/battle/0*, */api/battle/FFCCDD* |

## Technical Notes
* Front-end: JavaScript, AngularJS 1.6.9, Bootstrap 4.1.1, SASS 1.7.0
* Back-end: Java 1.8.0, Spring Boot 2.0.1, Drools 7.7.0
* Build system: Gradle 4.8
* Unit/Integration tests: Spock/Groovy
* Continuous Integration: Jenkins
* Code quality: SonarCloud
