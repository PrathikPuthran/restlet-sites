Jetty extension
===============

Introduction
============

This connector is based on the
[Jetty](http://www.mortbay.org/)
open-source web server. Jetty is popular and has a nice separation
between its HTTP protocol implementation and its support for the Servlet
API which led it to be the first HTTP server connector developed for the
Restlet.

Description
===========

This connector supports the following protocols: HTTP, HTTPS, AJP.

The list of supported specific parameters is available in the javadocs:

-   [Jetty common
    parameters](http://restlet.org/learn/javadocs/1.1/ext/com/noelios/restlet/ext/jetty/JettyServerHelper)
-   [HTTP specific
    parameters](http://restlet.org/learn/javadocs/1.1/ext/com/noelios/restlet/ext/jetty/HttpServerHelper)
-   [HTTPS specific
    parameters](http://restlet.org/learn/javadocs/1.1/ext/com/noelios/restlet/ext/jetty/HttpsServerHelper)

Here is the list of dependencies of this connector:

-   [Jetty
    6.1](http://www.mortbay.org/)
-   [Java Servlet
    2.5](http://java.sun.com/products/servlet/)

Usage example
=============

HTTPS
-----

For general information on Jetty HTTPS/SSL configuration, please read
[this
document](http://docs.codehaus.org/display/JETTY/How+to+configure+SSL).
For configuration of the connector in a Restlet component, you will need
to set some of the HTTPS parameters listed above, for example:

    Server server = myComponent.getServers().add(Protocol.HTTPS, 8183);
    server.getContext().getParameters().add("keystorePath", "<your-path>");
    server.getContext().getParameters().add("keystorePassword", "<your-password>");
    server.getContext().getParameters().add("keyPassword", "<your-password>");

