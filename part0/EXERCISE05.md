sequenceDiagram
    browser
    server

    browser: client goes to https://studies.cs.helsinki.fi/exampleapp/spa

    browser -> server: Get to https://studies.cs.helsinki.fi/exampleapp/spa

    server: receives request and handles it then sends a response

    server -> browser: server sends back a response containing an HTML file

    browser: after loading the page the browser makes 3 more request 

    browser -> server: GET to https://studies.cs.helsinki.fi/exampleapp/main.css

    browser -> server: GET to https://studies.cs.helsinki.fi/exampleapp/spa.js

    browser: executes JS file

    browser -> server: GET to https://studies.cs.helsinki.fi/exampleapp/data.json

    browser: executes callback function to show notes