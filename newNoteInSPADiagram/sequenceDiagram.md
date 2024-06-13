```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST /new_note
    Note right of browser: Send the data entered by the user as json
    activate server
    server-->>browser: data added
    deactivate server

    