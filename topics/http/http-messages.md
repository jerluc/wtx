# HTTP Messages

## Some examples

Though it's not very often that you need to interact directly with an HTTP message, it might be helpful to see what some examples of messages look like in order to understand more complicated interactions between HTTP clients and servers.

### A simple client request

A simple HTTP client might send a request message that looks something like this:

```text
GET /some-web-page.html HTTP/1.1
Host: jerluc.com
Accept: text/html
Cookie: chocolate_chip=yummy
```

#### Request line

In the first line of the HTTP request, `GET /some-web-page.html HTTP/1.1`, there are a few key parts worth noting:

1. `GET` refers to an HTTP _method:_ broadly speaking these describe what the HTTP client is trying to do with the data. In this case, `GET` means simply that the client is trying to download or "get" some data. There are plenty of other HTTP methods as well that each have their own meaning, such as `DELETE`, which you might have guessed means that a client wants to delete some data.
2. `/some-web-page.html` refers to the resource that the HTTP client wants to access. This is kind of like asking for a file in a folder on your computer \(though this is _not always_ the case\).
3. Lastly, the `HTTP/1.1` refers to the version of the HTTP protocol that the client is expecting to use. Most clients and servers today speak in HTTP 1.1 or 2.0, however in some cases an older client or server may only supporting older versions of HTTP. This is included in the client request message so that only supported versions can be responded to. For example, a client that speaks HTTP 2.0 would not necessarily be able to transfer data to/from a server that speaks HTTP 1.0.

#### Headers

The remaining lines are called HTTP _headers._

