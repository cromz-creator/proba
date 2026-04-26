# Parlamentarni izbori 2024 — Hrvatska

Interaktivna karta rezultata parlamentarnih izbora 2024.

## Struktura projekta

```
izbori-2024/
├── index.html              ← glavna stranica
├── data/
│   ├── granice.geojson     ← granice općina/gradova (~0.9 MB)
│   ├── opcine_index.json   ← mapping geo_key → filename
│   └── opcine/
│       └── *.json          ← detalji po svakoj općini (učitavaju se na klik)
└── README.md
```

## Kako pokrenuti lokalno

Potreban je HTTP server (ne možeš otvoriti index.html direktno iz filesystema zbog CORS-a).

**Python:**
```bash
cd izbori-2024
python3 -m http.server 8000
# Otvori http://localhost:8000
```

**Node.js:**
```bash
npx serve .
```

## GitHub Pages deployment

1. Napravi GitHub račun na https://github.com
2. Novi repozitorij: "New repository" → ime npr. `izbori-2024` → Public
3. Upload svih datoteka (index.html + cijeli data/ folder)
4. Settings → Pages → Source: "Deploy from branch" → main → / (root)
5. Stranica je dostupna na: `https://tvojeime.github.io/izbori-2024`

## Napomena o Zagrebu

Zagreb je podijeljen na 3 izborne zone (I., II., VI.).

