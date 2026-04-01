# Bibertbad Digital 🏊

Ein Aprilscherz von [OpenZirndorf](https://openzirndorf.de) – dem Civic-Tech-Projekt für Zirndorf, Bayern.

## Was ist das?

Eine einzelne HTML-Seite, die so tut, als wäre das Zirndorfer Freibad jetzt kostenlos digital verfügbar. Mit animiertem Schwimmbecken, Wassertemperatur-Anzeige und einem Flappy-Bird-Spiel – und am Ende die Auflösung: **April, April!**

Features:
- Bürger:innen-Check (nur Zirndorfer zahlen nichts 😉)
- Animiertes Becken mit CSS-Wellen, schwimmendem Enten-Emoji und Ripple-Effekt
- Flackernde Wassertemperatur (23–25°C)
- **Flappy-Becken-Spiel** – steuere eine Ente durch Bahnteiler, teile deinen Score
- Aprilscherz-Auflösung mit CTA zu openzirndorf.de und nativem Share-Button

## Deployment auf GitHub Pages

1. **Repo erstellen** auf GitHub (z.B. `openzirndorf/bad`)

2. **Dateien pushen:**
   ```bash
   git init
   git add .
   git commit -m "Bibertbad Digital – Aprilscherz"
   git remote add origin https://github.com/openzirndorf/bad.git
   git push -u origin main
   ```

3. **GitHub Pages aktivieren:**
   - Repository → Settings → Pages
   - Source: `Deploy from a branch`
   - Branch: `main` / `/ (root)`
   - Save

4. **Custom Domain eintragen:**
   - Unter Settings → Pages → Custom domain: `bad.openzirndorf.de`
   - Die `CNAME`-Datei ist bereits im Repo enthalten

5. **DNS-Eintrag beim Domain-Anbieter:**
   ```
   Typ:   CNAME
   Name:  bad
   Wert:  openzirndorf.github.io
   ```

Nach wenigen Minuten ist die Seite unter `https://bad.openzirndorf.de` erreichbar.

## Technik

- Nur `index.html` – kein Framework, kein Build-Step, keine Dependencies
- CSS + JS vollständig inline
- Mobile-first, getestet auf iOS Safari und Android Chrome
- Google Fonts: [Fraunces](https://fonts.google.com/specimen/Fraunces) + [DM Sans](https://fonts.google.com/specimen/DM+Sans)

---

Mit 💙 gemacht von OpenZirndorf · [openzirndorf.de](https://openzirndorf.de)
