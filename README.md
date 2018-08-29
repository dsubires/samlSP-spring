# samlSP-spring
Service provider compatible with the ECP profile based on spring-security-saml-1.0.4 RELEASE  https://repo.spring.io/list/release/org/springframework/security/extensions/spring-security-saml/

# samlSP-metadata-config
The IDP metadata is loaded directly through the URL specified in src/main/webapp/WEB-INF/securityContext.xml line 185.
The metadata of the SP are stored in src/main/resources/metadata/samlecp_sp.xml and the configuration in src/main/webapp/WEB-INF/securityContext.xml line 198.

This project can be built from the command line using the maven application or by eclipse and the plugin for maven (m2e) and deployed by tomcat

# Compilation

When building from sources compile whole project and install artifacts into your local Maven repository using:

$ gradlew build install

When using the release zip compile the sample application available in the sample directory using:

$ mvn package

# Deployment

You can start the application using command:

mvn tomcat7:run

Same can be achieved using gradle with:

gradlew tomcatRun

After startup the Spring SAML sample application will be available at http://localhost:8080/spring-security-saml2-sample

Alternatively you can deploy the war archive to your application server or container.
