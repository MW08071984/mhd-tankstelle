# MHD Management App - Tankstelle

Funktionen:
- Mitarbeiter-Login per Nummer + 4-stelligem Passwort
- Barcode-Scanner per Kamera
- automatische Produktdaten über OpenFoodFacts
- eigene Artikelbilder hochladen oder fotografieren
- MHD-Übersicht mit Warnungen
- Abschriftenliste
- Backwaren Tagesende
- iPhone/Android als Web-App/PWA

## Supabase einrichten
1. Supabase-Projekt erstellen.
2. SQL Editor öffnen und `SUPABASE_SQL.sql` ausführen.
3. Unter Authentication > Users Mitarbeiter anlegen:
   - `01@tankstelle.local`, Passwort z. B. `1234`
   - `02@tankstelle.local`, Passwort z. B. `5678`
4. Unter Project Settings > API kopieren:
   - Project URL
   - anon public key

## Vercel einrichten
1. Projekt zu GitHub hochladen oder als neues Projekt importieren.
2. In Vercel Project Settings > Environment Variables eintragen:
   - `VITE_SUPABASE_URL` = Supabase Project URL
   - `VITE_SUPABASE_ANON_KEY` = Supabase anon public key
3. Deploy starten.

## Lokal testen
```bash
npm install
npm run dev
```

## Personalwechsel
- Neuer Mitarbeiter: Supabase > Authentication > Users > Add user.
- Mitarbeiter entfernen: User löschen oder Passwort ändern.
- Nummer ändern: neuen User mit neuer Nummer anlegen.

## Hinweis zu Benachrichtigungen
Benachrichtigungen funktionieren am besten, wenn die App über HTTPS läuft und auf dem Handy zum Home-Bildschirm hinzugefügt wurde.
