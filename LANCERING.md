# agentpush.nl — livegang

De site staat online. Elke HTML-pagina heeft nog `noindex, nofollow`.
`robots.txt` laat crawlers toe, zodat die noindex gezien wordt. Niet blokkeren.

## Wat je aanzet

In deze vijf bestanden staat in de `<head>` deze tag (telkens de eerste robots-meta):

- `index.html`
- `meer.html`
- `plan.html`
- `review.html`
- `privacy.html`

Vervang

`<meta name="robots" content="noindex, nofollow">`

door

`<meta name="robots" content="index, follow">`

Daarna in Google Search Console de sitemap indienen: https://agentpush.nl/sitemap.xml

`robots.txt` hoeft daarvoor niet dicht. `Allow: /` en de sitemap-regel blijven.

Er is geen HTTP-header `X-Robots-Tag` in deze repo. Die niet via GitHub Pages toevoegen of aanzetten.

## Nog niet invullen tot Bob het aanlevert

- KvK-nummer. Staat bewust niet in de JSON-LD.
- Vestigingsadres. Staat bewust niet in de JSON-LD.
- Deelafbeelding `og.png` toont AgentPush Plan en AgentPush Review, niet AgentPush Run.

## Al klaar

- Titel, omschrijving, canonical, Open Graph en Twitter-card per pagina.
- JSON-LD: organisatie, AgentPush Plan, AgentPush Review, AgentPush Run, FAQ op meer.html, kruimelpad op de subpagina's.
- `sitemap.xml` en `llms.txt`.
