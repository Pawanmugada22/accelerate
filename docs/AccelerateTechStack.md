Accelerate Tech Stack
========================

Tech Stack :

> Hosting - Apache Tomcat/Nginx
> Rest Services - Spring Boot
> Database - Postgres
> Frontend - Angular
> Build - Gradle

Project Architecture :

The project is classified to three parts backend, frontend and both. The main or root project host the backend and frontend projects. In a way the root project will act as a bridge inbetween the frontend and backend project to get the final build which can be readily deployable in a server.

Root Project : **accelerate**
```
.
└── accelerate
    ├── build.gradle
    ├── client-sdlc
    ├── gradle
    ├── gradlew
    ├── gradlew.bat
    ├── README.md
    ├── sdlc
    └── settings.gradle
    
```
Front-end Project : **client-sdlc** 
```
client-sdlc
    ├── angular.json
    ├── browserslist
    ├── build.gradle
    ├── dist
    ├── e2e
    ├── gradle
    ├── gradlew
    ├── gradlew.bat
    ├── karma.conf.js
    ├── node_modules
    ├── package.json
    ├── package-lock.json
    ├── README.md
    ├── settings.gradle
    ├── src
    ├── tsconfig.app.json
    ├── tsconfig.json
    ├── tsconfig.spec.json
    └── tslint.json

```
Back-end Project : **sdlc**
```
sdlc
├── build
│   ├── classes
│   ├── generated
│   │   └── sources
│   ├── libs
│   │   └── sdlc-1.0.war
│   ├── resources
│   │   └── main
│   │       ├── application.properties
│   │       └── static
│   └── tmp
│       ├── bootWar
│       │   └── MANIFEST.MF
│       └── compileJava
├── build.gradle
├── gradle
│   └── wrapper
│       ├── gradle-wrapper.jar
│       └── gradle-wrapper.properties
├── gradlew
├── gradlew.bat
├── README.md
├── settings.gradle
└── src
    ├── main
    │   ├── java
    │   │   └── com
    │   │       └── accelerate
    │   │           └── sdlc
    │   │               ├── HelloSpring.java
    │   │               ├── SdlcApplication.java
    │   │               └── ServletInitializer.java
    │   └── resources
    │       ├── application.properties
    │       └── static
    └── test
        └── java
            └── com
                └── accelerate
                    └── sdlc
                        └── SdlcApplicationTests.java

```

Database Architecture :


