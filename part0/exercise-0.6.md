```mermaid

sequenceDiagram
        participant browser
        participant server

        browser->>+server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
        Note right of browser: Browser disables default reload of HTML
        Note right of browser: Browser creates new note, adds to list with notes.push(note), rerenders note list
        server-->>-browser: status code 201 created

```
