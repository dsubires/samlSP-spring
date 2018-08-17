# samlSP-spring
Service provider compatible with the ECP profile based on spring-security-saml-1.0.4 RELEASE 

# samlSP-metadata-config
The IDP metadata is loaded directly through the URL specified in src/main/webapp/WEB-INF/securityContext.xml line 185.
The metadata of the SP are stored in src/main/resources/metadata/samlecp_sp.xml and the configuration in src/main/webapp/WEB-INF/securityContext.xml line 198.

# Build & Deploy
This project can be built from the command line using the maven application or by eclipse and the plugin for maven (m2e) and deployed by tomcat

