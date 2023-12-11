sequenceDiagram
    browser
    server

    browser: client types into text field then clicks save button

    browser -> server: POST to https://studies.cs.helsinki.fi/exampleapp/new_note

    server: receives request and handles it then sends a response

    server -> browser: server sends back a redirect response

    browser: receives response to redirect to https://studies.cs.helsinki.fi/exampleapp/notes

    browser -> server: GET to https://studies.cs.helsinki.fi/exampleapp/notes

    browser: after reloading the page the browser makes 3 more request 

    browser -> server: GET to https://studies.cs.helsinki.fi/exampleapp/main.css 

    browser -> server: GET to https://studies.cs.helsinki.fi/exampleapp/main.js

    browser: executes JS file

    browser -> server: GET to https://studies.cs.helsinki.fi/exampleapp/data.json

    browser: executes callback function to show notes