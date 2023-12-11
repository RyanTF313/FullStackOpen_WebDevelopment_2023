sequenceDiagram
    browser
    server

    browser: client types into text field then clicks save button

    browser -> server: POST to https://studies.cs.helsinki.fi/exampleapp/new_note_spa

    server: receives request and handles it then sends a response

    server -> browser: server sends back a response message '''{"message":"note created"}'''

    browser: updates DOM with new message