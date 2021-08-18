Using WebSocket to build an interactive web application


Starting with Spring Initializr

- Adding Dependencies
  - The Spring Initializr does not provide everything you need in this case.

you need to add the following dependencies:


    implementation 'org.webjars:webjars-locator-core'
    implementation 'org.webjars:sockjs-client:1.0.2'
    implementation 'org.webjars:stomp-websocket:2.3.3'
    implementation 'org.webjars:bootstrap:3.3.7'
    implementation 'org.webjars:jquery:3.1.1-1'

- Create a Resource Representation Class

  - Now that you have set up the project and build system, you can create your STOMP message service.

  - Begin the process by thinking about service interactions.

  - The service will accept messages that contain a name in a STOMP message whose body is a JSON object


- Configure Spring for STOMP messaging


- Create a Browser Client


- Make the Application Executable

- Build an executable JAR

- Finally, Test the service
