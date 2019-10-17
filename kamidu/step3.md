Let's Take a look at the Project files.

# hello-world-config-project	
This is the ESB Config Project folder with the integration artifacts (synapse artifacts) for the HelloWorld service. This service consists of the following REST API:

HelloWorld.xml
<api context="/hello-world" name="HelloWorld" xmlns="http://ws.apache.org/ns/synapse">
    <resource methods="GET">
        <inSequence>
            <payloadFactory media-type="json">
                <format>{"Hello":"World"}</format>
                <args/>
            </payloadFactory>
            <respond/>
        </inSequence>
        <outSequence/>
        <faultSequence/>
    </resource>
</api>

# hello-world-config-projectCompositeApplication	
This is the Composite Application Project folder, which contains the packaged CAR file of the HelloWorld service.

# Dockerfile
	
This Docker configuration file is configured to build a Docker image for WSO2 Micro Integrator with the HelloWorld service.
 `Dockerfile`{{open}}
 
Note that this file is configured to use the community version of the WSO2 Micro Integrator base Docker image (from DockerHub). If you want to use the Micro Integrator that includes the latest product updates, you can update the image name in this Docker file as explained here.
