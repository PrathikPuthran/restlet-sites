HTTP Client extension
=====================

Introduction
============

This connector is based on [Apache Commons HTTP
client](http://jakarta.apache.org/commons/httpclient/).
It provides an HTTP and HTTPS client connector with advanced
multi-threading and connection reuse support.

Description
===========

As pointed out by the Apache HTTPClient tutorial it is crucial to read
entirely each response. It allows to release the underlying connection.
Not doing so may cause future requests to block. See [Apache HTTPClient
3.x
tutorial](http://jakarta.apache.org/httpcomponents/httpclient-3.x/tutorial.html).

This connector supports the following protocols: HTTP, HTTPS.

The list of supported specific parameters is available in the javadocs:

-   [HTTP client
    parameters](http://restlet.org/learn/javadocs/1.1/ext/com/noelios/restlet/ext/httpclient/HttpClientHelper.html)

Here is the list of dependencies of this connector:

-   [Apache Commons HTTP Client
    3.1](http://jakarta.apache.org/commons/httpclient/)
-   [Apache Commons Codec
    1.3](http://jakarta.apache.org/commons/codec/)
-   [Apache Commons Logging
    1.1](http://jakarta.apache.org/commons/logging/)

