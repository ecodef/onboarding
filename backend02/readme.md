# Hledání objektů ve čtvercové síti

## Požadavky

- Spring Application vytvořenou v public GitHub repository
- v Kotlinu
- pomocí Maven nebo Gradle

### úkol 1: REST API

#### vyhledávací služba
- `POST` metoda
- na URL `/demo/scan`
- na vstupu JSON objekt `{ "area": [[0,0,0],[0,1,0],[0,0,0]]}`
- vrací JSON objekt ` { "found": "true", "shape": "square"}`
- na vstupu je čtvercová síť, prázdné políčko 0, obsazené 1
- počet tvarů ve vstupní síti: 0 nebo 1 
- známé tvary: square, rectangle
- ostatní tvary: unknown
