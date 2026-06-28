# HTTP/HTTPS Overview — Simple Summary

**HTTP (Hypertext Transfer Protocol)** is the protocol used for communication between a **client** (such as a web browser) and a **server**. It follows a simple **request → response** model.

```text
Client (Browser)
       |
       |  HTTP Request
       v
     Server
       |
       |  HTTP Response
       v
Client (Browser)
```

The browser sends a **request** to the server, and the server processes it and sends back a **response**.

## The Two Parts of HTTP

HTTP communication always consists of **two parts**:

1. **Request** – Sent from the client to the server.
2. **Response** – Sent from the server back to the client.

---

# HTTP Request

A **request** contains information about what the client wants from the server.

Example:

```http
GET / HTTP/1.1
Host: jemyoung.com
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_5)
AppleWebKit/537.36 (KHTML, like Gecko)
Chrome/76.0.3809.132 Safari/537.36
Accept: text/html
Accept-Encoding: gzip, br
Accept-Language: en,en-US
```

### Parts of the Request

* **Request Line**

  * `GET` → HTTP method
  * `/` → Requested path
  * `HTTP/1.1` → HTTP version

* **Headers**

  * Extra information about the request, such as browser type, accepted content, language, and more.

---

## Common HTTP Request Headers

| Header            | Purpose                                                        |
| ----------------- | -------------------------------------------------------------- |
| `User-Agent`      | Identifies the browser or device making the request.           |
| `Accept`          | Specifies the content types the client can receive.            |
| `Accept-Language` | Indicates the user's preferred languages.                      |
| `Content-Type`    | Specifies the type of data being sent (e.g., JSON, HTML).      |
| `Set-Cookie`      | Used by the server to store cookies on the client.             |
| `X-*`             | Custom headers created by applications (e.g., `X-Request-ID`). |

---

# HTTP Response

After receiving the request, the server sends a **response**.

Example:

```http
HTTP/1.1 200 OK
Server: nginx/1.14.0 (Ubuntu)
Date: Wed, 25 Sep 2019 02:13:13 GMT
Content-Type: text/html; charset=utf-8
Content-Length: 12
```

### Parts of the Response

* **Status Line**

  * `HTTP/1.1` → HTTP version
  * `200` → Status code
  * `OK` → Status message

* **Headers**

  * Information about the response, such as server type, content type, and content length.

---

# HTTP Status Codes

A **status code** tells the client whether the request was successful or if an error occurred.

## Common Status Codes

| Status Code                 | Meaning                                                    |
| --------------------------- | ---------------------------------------------------------- |
| `200 OK`                    | The request was successful.                                |
| `301 Moved Permanently`     | The requested resource has permanently moved to a new URL. |
| `302 Found`                 | Temporary redirect to another URL.                         |
| `401 Unauthorized`          | Authentication is required or failed.                      |
| `500 Internal Server Error` | The server encountered an unexpected error.                |

---

## Status Code Categories

| Category | Meaning                 |
| -------- | ----------------------- |
| `1xx`    | Informational responses |
| `2xx`    | Successful requests     |
| `3xx`    | Redirection             |
| `4xx`    | Client errors           |
| `5xx`    | Server errors           |

---

# HTTPS

**HTTPS (Hypertext Transfer Protocol Secure)** is the secure version of HTTP.

Instead of sending data as plain text, HTTPS **encrypts** all communication between the browser and the server.

### Why HTTPS is Important

* Encrypts data sent over the internet.
* Prevents attackers from reading intercepted information.
* Protects sensitive data like:

  * Passwords
  * Credit card information
  * Personal details
* Helps prevent **Man-in-the-Middle (MITM)** attacks.

Without the correct encryption keys, intercepted data appears unreadable.

---

# HTTP vs HTTPS

| HTTP                        | HTTPS                                         |
| --------------------------- | --------------------------------------------- |
| Data is sent as plain text. | Data is encrypted before transmission.        |
| Less secure.                | Much more secure.                             |
| Vulnerable to interception. | Protects against intercepted data being read. |
| Uses port 80 (commonly).    | Uses port 443 (commonly).                     |

---

# Commands

There are **no terminal or shell commands** in these notes.

The examples shown are **HTTP messages**, not commands that you run in a terminal.

---

# Command Flags

There are **no command flags** because no terminal commands are used in these notes.

---

# One-Sentence Summary

**HTTP is the protocol that allows browsers and servers to communicate using requests and responses, while HTTPS adds encryption to make that communication secure and protect data from being intercepted.**
