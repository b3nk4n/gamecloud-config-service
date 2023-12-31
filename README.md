# GameCloud Config Service

This application is part of the GameCloud system and provides a configuration server.
The project was created based on a similar project of the
[Cloud Native Spring in Action](https://www.manning.com/books/cloud-native-spring-in-action) book
by [Thomas Vitale](https://www.thomasvitale.com).

## Useful Commands

| Gradle Command	         | Description                                                    |
|:---------------------------|:---------------------------------------------------------------|
| `./gradlew bootRun`        | Run the application.                                           |
| `./gradlew build`          | Build the application.                                         |
| `./gradlew test`           | Run tests.                                                     |
| `./gradlew bootJar`        | Package the application as a JAR.                              |
| `./gradlew bootBuildImage` | Package the application as a container image using Buildpacks. |

After building the application, you can also run it from the Java CLI:

```bash
java -jar build/libs/config-service-0.0.1-SNAPSHOT.jar
```

## Usage Examples

As a prerequisite for the following examples, you need [HTTPie](https://httpie.io/).
Alternatively, you can use `curl` as usual.

```bash
brew update
brew install httpie
```

```bash
http :8888/catalog-service/default
http :8888/catalog-service/prod
```

## Local development and tools

Check out the rather similar command for GameCloud [catalog-service](https://github.com/b3nk4n/gamecloud-catalog-service#local-development-and-tools).
