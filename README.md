# MHD Tankstelle App - finale Version

Enthalten:
- Mitarbeiter Login mit Nummer + 4-stelligem Passwort
- Barcode Scanner
- automatische Produktdaten/Bilder über OpenFoodFacts
- eigene Artikelbilder hochladen
- MHD Dashboard
- Abschriftenliste
- Backwaren Tagesende
- Browser/PWA Benachrichtigungen

## Supabase
SQL Editor öffnen und `database.sql` ausführen.
Mitarbeiter als User anlegen, z.B. `01@tankstelle.local` mit Passwort `1234`.

## Vercel
Environment Variables:
- VITE_SUPABASE_URL
- VITE_SUPABASE_ANON_KEY

Danach deployen.
