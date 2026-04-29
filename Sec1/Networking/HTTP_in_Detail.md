# HTTP in Detail 

## Overview

This lab introduces the **HTTP/HTTPS protocol**, which underpins communication between clients and web servers. It builds on foundational knowledge and explores how web requests and responses are structured, along with their relevance in real-world scenarios.

---

## HTTP vs HTTPS

- **HTTP (HyperText Transfer Protocol)** is used for transferring data such as HTML and images between a client and a web server  
- **HTTPS** is the secure version, using encryption (TLS) to protect data in transit  

A padlock icon in the browser indicates that HTTPS is in use, helping ensure that communication is encrypted and less susceptible to interception.

---

## URL Structure

A **URL (Uniform Resource Locator)** acts as an instruction to locate a resource on the internet.

It consists of several components:

- **Scheme** – Protocol used (e.g., HTTP/HTTPS)  
- **User** – Optional authentication information  
- **Host** – Domain or IP address  
- **Port** – Communication port (default 80 for HTTP, 443 for HTTPS)  
- **Path** – Location of the resource  
- **Query String** – Additional parameters  
- **Fragment** – Directs to a specific part of a webpage  

The concept of a *fragment* was new and allows users to jump directly to a section within a page.

---

## HTTP Requests & Responses

Communication between a client and server follows a request/response model:

### Request
Sent by the client to the server

### Response
Returned by the server with:
- requested resource  
- status code  
- headers  

Key response headers include:
- **Content-Type** – Type of data returned  
- **Content-Length** – Size of the response  

These fields can be useful during investigations to understand what data is being transmitted.

---

## HTTP Methods

HTTP methods define the intended action of a request:

- **GET** – Retrieve data  
- **POST** – Send data to the server  
- **PUT** – Update existing data  
- **DELETE** – Remove data  

These are important when analysing traffic, as unusual or unexpected methods may indicate suspicious behaviour.

---

## HTTP Status Codes

Status codes indicate the result of a request:

- **200–299** → Success  
- **300–399** → Redirection  
- **400–499** → Client errors (e.g., 403 Forbidden, 404 Not Found)  
- **500–599** → Server errors  

While memorisation is not essential, recognising common codes (such as 403 and 404) is useful. Over time, familiarity improves through exposure.

---

## Headers

Headers provide additional information about requests and responses.

Example:
- **User-Agent** – Identifies the client making the request  

Headers can reveal useful details during analysis, such as:
- browser type  
- scripts or automated tools  
- unusual or suspicious behaviour  

---

## Cookies

Cookies are small pieces of data stored on a client device:

- Sent by the server using **Set-Cookie**  
- Returned by the client in future requests  

They allow websites to maintain state, as HTTP itself is **stateless**.

From a security perspective:
- Cookies may contain session tokens  
- Poorly secured cookies can be targeted or hijacked  

---

## Practical Exercise

The lab included hands-on interaction with HTTP requests, allowing observation of:

- request structure  
- response headers  
- status codes  

This helped reinforce how web communication functions in practice.
![POST_Request](Screenshots/THMHTTPinDetail.png)

---

## Key Takeaways

- HTTP/HTTPS underpin all web communication  
- Requests and responses contain valuable information for analysis  
- Methods and status codes help identify behaviour and outcomes  
- Headers and cookies can reveal important context about users and systems  

---

## SOC Relevance

Understanding HTTP is essential for security roles because:

- Web traffic is a primary attack surface  
- Suspicious requests (e.g., unusual methods or headers) can indicate malicious activity  
- Status codes and response data help identify errors, misconfigurations, or probing behaviour  
- Cookies and session handling are common targets in web-based attacks  

---

## Reflection

This lab expanded on existing knowledge and introduced more detailed concepts such as HTTP methods and URL structure. It also highlighted how HTTP data can be analysed from a security perspective, forming a foundation for understanding web-based attacks and investigations.
