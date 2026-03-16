# cheapgear.dk – Growth & Driftplan

## Kontekst
- Fokus: få Partner-ads produkter korrekt ind i WooCommerce, sikre stabil import/cron, løfte indhold & SEO, forbedre performance og etablere rapportering.
- Bilag: `data/affiliate-shops.csv` (liste over kataloger/fora m.m. fra Ferieboligsiden-projektet) + fotonoter fra terminalen (cheapgear login).

## Workstreams & delmål

### 1. Import & cron-kontrol
- [ ] Kortlæg alle WP All Import jobs (navn, hyppighed, sidste kørsel, fejl).
- [ ] Rens køer + duplikerede jobs. Sørg for at alle relevante jobs står til "weekly" som ønsket.
- [ ] Opdatér WP All Import Pro + addons til nyeste version.
- [ ] Dokumentér rækkefølgen for import (Partner-ads CSV → WooCommerce → cron/queue).
- Afhængigheder: WordPress admin-login + evt. SSH for cron log.

### 2. Produktkvalitet & struktur
- [ ] Tjek at Partner-ads kategorier mappes korrekt til WooCommerce kategorier.
- [ ] Udfyld/berig felter ("Kommission", pris, stok, attributter) i importtemplate.
- [ ] Opsæt bundlinks/sektioner i templates så produktkort automatisk får CTA + deeplinks.
- Afhængigheder: Mapping-dokument + adgang til importskabelon.

### 3. Indhold & SEO
- [ ] Liste over kernesider (lande/temaer) der mangler/skal opdateres.
- [ ] Plan for artikler (guides/tests) med interne links til produkter.
- [ ] Tjek Yoast/SEO-plugin indstillinger + XML-sitemap.
- Afhængigheder: CMS-adgang, søgeordsdata.

### 4. Teknisk performance
- [ ] Core Web Vitals-måling (PageSpeed eller CrUX) og action plan (cache, billedkomprimering, lazyload).
- [ ] CDN/caching-tjek (fx Cloudflare/LSCache?).
- Afhængigheder: Hosting login / WP plugin adgang.

### 5. Tracking & rapportering
- [ ] Bekræft GA4 + evt. Server-side tagging.
- [ ] Sæt Looker/Google Sheets rapport op med importstatus + trafik/konverteringer.
- [ ] UTM-skabeloner til Partner-ads og outbound links.
- Afhængigheder: GA4-adgang, evt. Tag Manager.

### 6. Trafik-boost & kataloger
- [x] Import af CSV liste til workspace (`data/affiliate-shops.csv`).
- [ ] Prioritér domæner (DR, kategori, loginstatus) → se `outreach-priorities.md`.
- [ ] Definér first wave: høj-DR lister + relevante DK fora/blogs.
- [ ] Status-tracking (oprettet, pending, kræver manuelt review).
- Afhængigheder: Oprettede konti (se noter i CSV), evt. dedikeret e-mail.

## Næste skridt (foreslået rækkefølge)
1. **Adgang** – få WP/hosting/GA4-login så de tekniske workstreams kan påbegyndes.
2. **Import-audit** – når adgang er klar, kør fuld gennemgang af WP All Import jobs og dokumentér fund.
3. **Content/SEO backlog** – udtræk nuværende URL-struktur + identificér huller.
4. **Tracking blueprint** – skitser målepunkter + dashboards.
5. **Katalog outreach** – begynd med top 10 DR-domæner, log status i et ark (kan lægges i `projects/cheapgear/outreach-status.csv`).
6. **Brand & SoMe** – definér tone of voice, opret sociale profiler (X, IG, TikTok, YouTube Shorts) og dokumentér logins i en krypteret note.

## Åbne spørgsmål / behov
- Hvilken e-mail skal bruges til nye profiler (fx support@ / info@) + hvor hentes credentials?
- Er der staging-miljø til tests, eller skal vi arbejde direkte på live?
- Brandretning: særlige no-go’s/farver/positionering?
- Hvilke rapporter/data ønsker du løbende (ugentlig opsummering, dashboard osv.)?

## Log
- 2026-03-14: Oprettet projektmappe, importeret affiliate-listen, genereret top-25 DR prioriteringsoversigt.
- 2026-03-14 17:00: Rolle udvidet til fuld strategi/CEO, SoMe-plan tilføjet.
- 2026-03-14 18:20: Konfigureret info@grafiisk.dk (IMAP/SMTP) og sendt intro-mail til Kevin m/cc Frank.
- 2026-03-14 18:25: Tilføjet info@cheapgear.dk mailbox (server1.designrus.dk).
- 2026-03-14 18:30: Opdateret hero-tekst + topbillede på cheapgear.dk (WP side 138) for at vise adgang.
