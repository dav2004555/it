# Exercise 0.6
```md
# Exercise 0.6 – New SPA note diagram
```mermaid
sequenceDiagram
    participant browser
    participant server

    Note right of browser: User writes note and presses Save
    browser->>server: POST /new_note_spa (JSON with note)
    server-->>browser: 201 Created

    Note right of browser: JS updates UI without reloading page
