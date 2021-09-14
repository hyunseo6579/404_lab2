# 404_lab2 Answers

1. It is specified by passing in SOCK_STREAM as socket type into socket.socket() function.
   * resource 1: https://docs.python.org/3/library/socket.html#socket.SOCK_STREAM
   * resource 2: https://stackoverflow.com/questions/5815675/what-is-sock-dgram-and-sock-stream

2. Client sockets call connect() while server sockets call listen() and waits for connect() which then calls accept().
   * resource: https://stackoverflow.com/questions/774571/server-vs-client-socket-low-level-details

3. By setting socket option to allow reuse of address by calling ```s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)```

4. From the server side, I get the information about the ip address and port number of the incoming connections.

5. The return value is a byte object representing the data received where maximum amount of data received at once is the buffer size that is specified by ```buffer_size```.
   * resource: https://docs.python.org/3/library/socket.html#socket.socket.connect

6. https://github.com/hyunseo6579/404_lab2/
