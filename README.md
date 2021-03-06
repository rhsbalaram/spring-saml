OAuth 2.0 Login Sample
This guide provides instructions on setting up this SAML 2.0 Login sample application.

The sample application uses Spring Boot and the spring-security-saml2-service-provider module which is new in Spring Security 5.2.

Goals
saml2Login() provides a very simple implementation of a Service Provider that can receive a SAML 2.0 Response via the HTTP-POST and HTTP-REDIRECT bindings against the SimpleSAMLphp SAML 2.0 reference implementation.

The following features are implemented in the MVP:

Receive and validate a SAML 2.0 Response containing an assertion, and create a corresponding authentication in Spring Security

Send a SAML 2.0 AuthNRequest to an Identity Provider

Provide a framework for components used in SAML 2.0 authentication that can be swapped by configuration

Work against the SimpleSAMLphp reference implementation

Run the Sample
Start up the Sample Boot Application
 ./gradlew :spring-security-samples-boot-saml2login:bootRun
Open a Browser
http://localhost:8080/

You will be redirect to the SimpleSAMLphp IDP

Type in your credentials
User: user
Password: password