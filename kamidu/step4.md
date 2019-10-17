Let's create a docker image with WSO2 migro intregrator and the sample artifacts.
`docker build -t hello_world_docker_image .` {{execute}}

Above command executes the following tasks:

* The base Docker image of WSO2 Micro Integrator is downloaded from DockerHub and a custom, deployable Docker image of the Micro Integrator is created in a Docker container.
* The CAR file with the integration artifacts that define the HelloWorld service is deployed.