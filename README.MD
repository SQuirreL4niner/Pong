# Pong Project

This project consists of a front end ui, relay server to consume external api, back end to create REST api, database to persist data, docker images to
contain layered services, and a cloud server to host the app

## Getting Started



### Prerequisites

What things you need to install the software and how to install them

```
Frameworks & Languages: Java 8, gradle, node, npm, docker, docker compose, jasmine, Lombok, git
```

```
IDE's: Spring Tool Suite (STS), Atom, VIM
```

### Installing

To install UI Client and Node locally (from the service root)-

  `$ npm install `

To install the back end API -

  `$ gradle clean build `



## Running the tests

To run back end unit tests run the following command -

  `$ gradle clean build `

To run ui tests run -

  `$ npm test `


## Local Deployment

From Client and Node directories w/out docker for UI developing -
  `$ npm start`

From Pong-Api directory using docker and remote mongodb -
  `$ sudo docker run -p 8080:8080 pong-api`

From project root using docker compose -
  `$ sudo docker-compose up`

## Remote Deployment

  From Client, Node and Pong-Api directories with docker to Heroku -
    `$ sudo docker build -t <name of service deployment> . `

    `$ sudo docker tag <name of service deployment> registry.heroku.com/<name of service deployment/web `

    `$ sudo docker push registry.heroku.com/<name of service deployment>/web
 `

## Built With

* [ReactJS](https://reactjs.org/) - The web ui library used
* [Material-UI](http://www.material-ui.com/#/) - Material library for UI
* [Axios](https://github.com/axios/axios) - Post library used for UI
* [React CLI](https://github.com/facebookincubator/create-react-app) - React CLI
* [Webpack](https://webpack.js.org/) - UI Bundler
* [NPM](https://www.npmjs.com/) - Package manager and task runner for UI and Node Server
* [Express](https://expressjs.com/) - Relay server framework
* [Node](https://nodejs.org/en/) - JS Runtime for relay server
* [Jasmine](https://jasmine.github.io/) - UI unit testing framework
* [Karma](https://karma-runner.github.io/1.0/index.html) - UI unit testing runner
* [Phantom.js](http://phantomjs.org/) - Header browser for UI unit testing
* [cors.js](https://github.com/expressjs/cors) - Cors middleware for relay server
* [Spring Reactor](https://projectreactor.io/) - Spring RX for streams/events
* [Spring Boot](https://projects.spring.io/spring-boot/) - Spring framework for bootstraping and developing back end
* [Lombok](https://projectlombok.org/) - Back End pojo enhancement/plugin for STS
* [Java 8](http://www.oracle.com/technetwork/java/javase/overview/java8-2100321.html) - UI Dev Language
* [Junit](http://junit.org/junit5/) - Unit testing for back end
* [Mockito](http://site.mockito.org/) - Mock data library for back end unit testing
* [Gradle](https://gradle.org/) - Dependency management and build tool for back end
* [Mongo](https://www.mongodb.com/) - Database
* [Docker](https://www.docker.com/) - Linux image containerization for service layers
* [Docker Compose](https://docs.docker.com/compose/) - Orchestrator for Docker
* [Heroku](https://dashboard.heroku.com/) - Cloud platform as a service for app


## Authors

* **Brandon Maciel** - *Full Stack* - [Eprojex.network](http://eprojex.net)

* **Jeff Goyette** - *Technical Advice on Spring Reactor and Docker Compose* - (jgoyette.jg@gmail.com)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

Special thanks to Stack Overflow as usual!!!!!!!!!!!
