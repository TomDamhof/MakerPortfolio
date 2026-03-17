# Tom Damhof — Maker Portfolio

## 📁 Bestandsstructuur

```
portfolio/
├── index.html               ← Homepage (niet aanpassen)
├── projects.json            ← ⭐ HIER voeg je projecten toe
├── README.md                ← Dit bestand
│
├── projects/
│   ├── project-template.html   ← ⭐ Kopieer dit voor elk nieuw project
│   ├── custom-enclosure.html   ← Voorbeeld project
│   ├── arduino-sensorstation.html
│   └── ...                     ← Jouw eigen projecten
│
└── images/
    ├── custom-enclosure-thumb.jpg   ← Thumbnail voor homepage
    ├── custom-enclosure-1.jpg       ← Foto's voor projectpagina
    └── ...                          ← Al je foto's
```

---

## ➕ Nieuw project toevoegen

### Stap 1 — Kopieer het template
Kopieer `projects/project-template.html` naar een nieuw bestand:
```
projects/mijn-nieuw-project.html
```

### Stap 2 — Vul het template in
Open het nieuwe bestand en zoek alle plekken met `← EDIT →`.
Vul in:
- Titel, tag, jaar
- Samenvatting (NL + EN)
- Foto's (zie stap 3)
- Uitgebreide beschrijving
- Materialen & tools

### Stap 3 — Voeg foto's toe
Zet al je foto's in de `/images/` map.
Gebruik duidelijke namen, bijv:
```
images/mijn-project-thumb.jpg    ← thumbnail (homepage kaart)
images/mijn-project-1.jpg        ← foto 1 op projectpagina
images/mijn-project-2.jpg        ← foto 2
```

### Stap 4 — Registreer in projects.json
Open `projects.json` en voeg een regel toe:

```json
{
  "file": "projects/mijn-nieuw-project.html",
  "title": "Mijn Project",
  "tag": "3D Printing",
  "description": "Korte beschrijving voor de homepage kaart.",
  "description_en": "Short description for the homepage card.",
  "thumb": "images/mijn-project-thumb.jpg",
  "year": "2025"
}
```

Dat is alles! De homepage laadt automatisch je nieuwe project.

---

## 🖼️ Foto layouts in het template

Het template heeft 4 layouts om uit te kiezen. Verwijder de layouts die je niet gebruikt:

| Layout | Beschrijving |
|--------|-------------|
| `gallery-a` | 1 grote links + 2 kleine rechts (aanbevolen) |
| `gallery-b` | 3 gelijke kolommen |
| `gallery-c` | 1 brede foto |
| `gallery-d` | 2 gelijke kolommen |

Je kunt ook een **YouTube video** embedden — zie het commentaar in het template.

---

## 🌐 GitHub Pages

1. Push alle bestanden naar je GitHub repo
2. Ga naar Settings → Pages → Source: main branch / root
3. Je portfolio is live op `https://jouwgebruikersnaam.github.io/repo-naam`
