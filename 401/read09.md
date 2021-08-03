
# HTTP Request Lifecycle 
HyperText Transfer Protocol The communications protocol used to connect to Web servers on the Internet or on a local network (intranet). The primary function of HTTP is to establish a connection with the server and send HTML pages back to the user's browser. It is also used to download data from the server either to the browser or to any requesting application that uses HTTP.

1. Local Processing: browser extracts the "scheme"/protocol,consist of host, and optional port number, resource path, and query strings .

2. resolving an IP from a DNS server.
+  If the cache lookup fails the browser will fire off DNS request by UDP .
+ Whenever the packet hits a piece of networking equipment, the device uses a routing table to determine which other device it is connected to that is most likely situated along the shortest path to the destination.
+ Once your request arrives at your configured DNS server, the server looks for the address associated with the requested hostname. 

3. Establish a TCP Connection:  since the request is sent over TCP6, which is a transport layer protocol like UDP, the client must open a TCP connection.

4. Send an HTTP Request: now that the client has an IP address and a TCP connection, it can finally send an HTTP request, The request is made up of a "request line", request header, and a body. 

![http](https://lh3.googleusercontent.com/proxy/HxcnrU9RisExWecWoTS2XPcIcQOq9dCKKacHtVLMs-6N6E6yy9kLo_KmC5U-FnWTWeaJNSSxUuKxSmdRiBVGOha_a3tPwNKuj5uCEKzpNDLMxYR0virJzloilFUI0HMoD-3lMNzC)

starting from JDK 11, java provides a new API for HTTP requests, replacing the HttpUrlConnection with HttpClientAPI .

#### HttpUrlConnection
HttpUrlConnection class is used to perform basic HTTP requests without the use of any additional libraries, but this way has a disadvantage which is using this method are that the code can be more cumbersome than other HTTP libraries and that it does not provide more advanced functionalities such as dedicated methods for adding headers or authentication.

####  Creating a Request
+ we create an HttpUrlConnection instance ising the openConnection() method of the URL class, this method only creates a connection object but doesnt establish the connection.

+ The HttpUrlConnection class is used for all types of requests by setting the requestMethod attribute to one of the values: GET, POST, HEAD, OPTIONS, PUT, DELETE, TRACE.

```
URL url = new URL("http://example.com");
HttpURLConnection con = (HttpURLConnection) url.openConnection();
con.setRequestMethod("GET");
```

















## [BACK](../README.md)