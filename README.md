# GraalVM helloworld with Docker
This is a simple HelloWorld application that's being compiled to a native executable with graalVM using docker.

I did not found a working example, and after trying endlessly I found this working solution, so I decided to keep it here for future reference.

## Application
The application has only a ``/hello`` endpoint, returning a simple String.

## Dockerfile
* stage 1: build the native image
* stage 2: start from a very slim linux image, copy the native image from stage 1 and run it
