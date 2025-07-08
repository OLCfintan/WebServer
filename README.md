----------------------- Web Server Structure --------------------------

We need to implement :
----------------------

    => WebServer that listen on a prof , accept clients and process
        requests.
    => Request part that parses raw http data into method headers
        URL body ...
    =>Response part that builds correct HTTP response (200 ok,
        404,...).
    =>CGIHandler that execute CGI programs and return their
            output as HTTP response.

-----------------------------------------------------------------------

What is a web server ?
----------------------

    -A web server is a program (or a computer running that program)
        that receives HTTP request from clients (like web browsers)
        process them , and sends back to HTTP response.

    For EXP :
        <CHROME> to <WEBSERVER> : give index.html
        <WEBSERVER> to <CHROME> : webserver looks in it;s storage finds
            index.html and sends it back with 200 ok or 404 not found
            if deos not exist.

What a websever do ?
--------------------

    1- Listen on a port (wait for the client to connect).
    2-Accept client connection(When the client connects the server
        accept it).
    3-Read the request(recieves HTTP request).
    4-Parse the request.
    5-Generate a response.
    6-Send response.
    7-Close connection.

Types of web servers ?
----------------------

    1-Static servers :

        Like ngnix Apache ( Serves only files).

    2-Dynamic servers :

        Flask, Node.js, GCIbased ( Runs programs to generate content ).

What is CGI ?
-------------

    A way for the webserver to run external programs/scripts
        and use their output as the HTTP response.






















