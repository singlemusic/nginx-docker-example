# nginx-docker-example

This is an example project demonstrating a maven-based
project that builds a simple nginx docker image.

## Building
This project includes the [maven-wrapper](https://github.com/takari/maven-wrapper) so you only need the JDK installed to build.

To create the docker image run:
```
./mvnw clean install
```

## Running

To start the nginx image that was built, run:

```
./mvnw docker:start
```

If you see an error about a missing network run:
```
docker network create --attachable local-network
```
alternatively, you can change the network defined in the
`pom.xml` configuration to one that already exists on
your system.

Navigate to `http://localhost:8080` to see the page served
up from the nginx container.