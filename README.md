# **Docker Multi-Stage Builds**

This repository contains multiple Dockerfiles that demonstrate the use of multi-stage builds to reduce the size of Docker images.

## **Overview**

Docker multi-stage builds allow you to use multiple FROM statements in a single Dockerfile. Each FROM statement can use a different base image and can copy artifacts from one stage to another, leaving behind anything not explicitly copied. This can significantly reduce the size of the final image.

In this repository, you’ll find several Dockerfiles that show different combinations of instructions to achieve smaller image sizes using multi-stage builds.

## **Usage**

To build an image using one of the Dockerfiles in this repository, navigate to the directory containing the Dockerfile and run the following command:

``` docker build -t my-image . ```     Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy.



This will build an image using the specified Dockerfile and tag it as my-image. You can then run a container using this image with the following command:

``` docker run my-image ```           Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy.


## **Conclusion**

Docker multi-stage builds are a powerful tool for reducing the size of your images. By using multiple FROM statements and selectively copying artifacts between stages, you can create smaller, more efficient images. This repository provides several examples of how to achieve this using different combinations of instructions in your Dockerfiles.
