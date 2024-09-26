# part0

```mermaid
  sequenceDiagram;
      participant user
      participant browser
      participant server

user->>browser: User submits a new note via form
browser->> sends the user input in form of a request to the server (post https://studies.cs.helsinki.fi/exampleapp/new_note)
server->> responds with a HTTP status code 302 . This is a URL redirect.
server->> asks the browser to perform a HTTP Get request to the address which is in the headers location.
browser->> reloads the Notes page. ( 3 more HTTP requests for css, js and data.json. 

```
