```mermaid
    title Create a new note

    browser->server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note
    server-->browser: URL redirect
    browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes
    server-->browser: HTML content

    note over browser:
    After the HTTP POST
    request, the server response
    with an URL redirect
    end note


    browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css
    server-->browser: main.css
    browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.js
    server-->browser: main.js
    browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json
    server-->browser: data.json

    note over browser:
    The reload causes more
    request to load the
    resources
    end note
```
