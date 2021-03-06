# come2help Server

<a href="http://come2.help">come2.help</a> is a project for recruiting and coordinating volunteer people.
Possible scenarios are flooding or coordinating support for political refugees.

## Content and Usage

This is only a REST API for the server. The frontend is not part of this repository. For usage please care about the
LICENSE file.
 
## Setup

1. Fork the repository for development. Implementations can be submitted by a Pull-Request.

2. Clone the repository to a local directory.

3. Import it to a IDE (e.g. IntelliJ) of your choice (or use vim).

4. Add a local mysql user and database, the default data can be found in application.properties. Do not use this
authentication data for production use.

5. First build a jar file, this can be done with:
<pre>mvn package</pre>

6. Execute the binary:
<pre>java -jar target/come2help-server-0.0.1-SNAPSHOT.jar</pre>

7. Execute a request against the REST-API. For example use a REST-Client extension for your browser. For testing you can
use the following curl command line:
<pre>curl http://localhost:8080/users/1</pre>
The result should be the user with the ID 1 (if there is no one, create it with PUT and the URI http://localhost:8080/users.
Data can be transmitted as JSON.

## Contact

For further contact mail valentin.zickner(at)helfenkannjeder(dot)de, visit http://come2.help/ or create a ticket.