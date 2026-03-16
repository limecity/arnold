# Grafiisk.dk – Prisberegner (wireframe + logik)

## Formål
- Give besøgende et hurtigt estimat på en ny hjemmeside.
- Opsamle leads (navn, e-mail, telefon) efter de har set prisoverslag.
- Skabe gennemsigtighed og differentiere mellem pakker/tilkøb.

## Flow (wireframe i tekst)
1. **Hero**: Kort intro + USP + “Beregn pris” CTA.
2. **Trin 1 – Projektinfo**
   - Vælg type: Landingpage / Business-site / Webshop / Special.
   - Vælg antal sider/sektioner (slider eller dropdown).
3. **Trin 2 – Funktioner**
   - CMS (inkluderet) – checkbox til specielle krav.
   - Blog/nyheder, Booking, Flersproget, E-commerce, Integrationer.
   - Indhold: Skal vi levere tekst/foto? (ja/nej).
4. **Trin 3 – Servicepakker**
   - Basis (design + implementering).
   - Plus (inkl. copy, SEO-basis, support).
   - Premium (plus hosting, vedligehold osv.).
5. **Opsummering**
   - Viser prisinterval (fx 35.000–45.000 DKK) med forklaring.
   - Formular til kontakt (navn, e-mail, telefon, besked).
   - CTA: “Book møde” / “Få tilbud”.
6. **Trust-sektion**
   - Kunder/logoer/testimonials.

## Prislogik (udkast)
- Grundpris pr. type:
  - Landingpage: 15.000 DKK
  - Business-site (op til 8 sider): 28.000 DKK
  - Webshop (op til 50 produkter): 45.000 DKK
  - Special (skriv til os) – viser “fra 60.000 DKK”.
- Side/sektion-tillæg: 1.200 DKK pr. ekstra side over basis.
- Funktionstillæg:
  - Blog/nyheder: 3.000 DKK
  - Booking/kalender: 4.500 DKK
  - Flersproget: 5.000 DKK
  - E-commerce (ud over base): 8.000 DKK
  - Integrationer/API: 7.500 DKK
  - Indholdsproduktion (tekst/foto): 6.000 DKK
- Servicepakker (multiplikatorer):
  - Basis: x1,0
  - Plus: x1,15 (inkl. copy + SEO + support)
  - Premium: x1,35 (inkl. hosting, vedligehold, løbende optimeringer)

Output: Pris vises som interval ±10 % for transparens.

## UX-noter
- Brug multi-step form (progress bar).
- Mobile-first: store knapper, tydelige kort.
- Efter beregning: vis pris + opfordring til at booke møde.
- Mulighed for at sende pdf-resumé på e-mail (option).

## Næste skridt
1. Godkend/justér pakker + prisinterval.
2. Byg custom plugin med shortcode `[grafiisk_prisberegner]`.
3. Styling i child theme (match brand).
4. Opsamling i CRM (e-mail notifikationer).
