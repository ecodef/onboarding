# Zabezpečené REST API

## Požadavky

- Spring Application vytvořenou v public GitHub repository
- v Kotlinu
- pomocí Maven nebo Gradle

### úkol 1: REST API

#### první služba
- `GET` metoda
- na URL `/demo/now`
- bez vstupních parametrů
- vrací JSON objekt `{ date: "dd.mm.yyyy", time: "hh:mi:ss,nnn", timeZone: "standard pacific time"}`

#### druhá služba
- `GET` metoda
- na URL `/demo/whoami`
- bez vstupních parametrů
- vrací JSON objekt `{ subject: "Vlasta Burian" }`

### úkol 2: zabezpečení REST API pomocí Bearer Tokenu
- Pomocí Springu vytvořit oAuthServer
- Z něj získat Bearer token třeba pomocí `curl -X POST username:password@localhost:9000/oauth2/token`
- Následně s tímto tokenem v hlavičce zavolat `GET /demo/whoami` z úkolu 1
- Místo 'Vlasta Burian' se vrátí skutečný subject z tokenu
