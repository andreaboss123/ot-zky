# Maturitní otázky – Účetnictví (ČR)

## 📄 Kde najdu hotový dokument? / Where can I find the done document?

**✅ Dokument je připraven!** 

### Jak stáhnout dokument / How to download the document:

**Krok 1:** Otevřete složku `output` v tomto repozitáři  
**Step 1:** Open the `output` folder in this repository

**Krok 2:** Klikněte na soubor `maturitni_otazky_ucetnictvi.docx`  
**Step 2:** Click on the file `maturitni_otazky_ucetnictvi.docx`

**Krok 3:** Stiskněte tlačítko "Download" (nebo "Stáhnout") v pravém horním rohu  
**Step 3:** Press the "Download" button in the top right corner

### Přímá cesta k souboru / Direct path to the file:

```
ot-zky/
└── output/
    └── maturitni_otazky_ucetnictvi.docx  ← ⭐ DOKUMENT JE TADY / THE DOCUMENT IS HERE
```

**GitHub URL:** [Click here to view the file on GitHub](../../tree/main/output)

Nebo použijte tento přímý odkaz k souboru:  
Or use this direct link to the file:
- `output/maturitni_otazky_ucetnictvi.docx` (43 KB)

---

## Struktura repozitáře / Repository Structure

**Aktuální struktura / Current structure:**

```
ot-zky/
├── output/                           ← 📂 Vygenerované dokumenty / Generated documents
│   └── maturitni_otazky_ucetnictvi.docx  (43 KB)
├── docs/
│   └── src/
│       └── otazky.md                 ← 📝 Zdrojový obsah (22 kapitol) / Source content
├── scripts/
│   └── generate_docx.py              ← 🐍 Python skript pro generování / Generation script
├── .github/
│   └── workflows/
│       └── generate-docx.yml         ← ⚙️ GitHub Actions workflow
├── requirements.txt                  ← 📦 Python závislosti / Dependencies
└── README.md                         ← 📖 Tento soubor / This file
```

---

## Formát dokumentu / Document Format

- **Font:** Times New Roman 12
- **Řádkování / Line spacing:** 1.5
- **Okraje / Margins:** 2.5 cm
- **Struktura / Structure:**
  - Titulní strana
  - Obsah
  - 22 otázek - každá otázka a odpověď na samostatných stránkách:
    - **Otázka** (levá/lichá stránka): Pouze název otázky (vycentrovaný)
    - **Odpověď** (pravá/sudá stránka): Kompletní odpověď na otázku
  - Číslování stránek od 1. kapitoly

---

## Status

- [x] Vytvořena struktura repozitáře
- [x] Napsán obsah otázek (22 kapitol)
- [x] Vytvořen generovací skript
- [x] Nastaveno GitHub Actions
- [x] Vygenerován finální dokument

**✅ Finální dokument je k dispozici v adresáři `output/maturitni_otazky_ucetnictvi.docx`**

---

## Jak vygenerovat dokument znovu / How to regenerate the document

Pokud chcete upravit obsah a vygenerovat dokument znovu:

1. **Upravte otázky** v souboru `docs/src/otazky.md`
2. **Spusťte generátor:**
   ```bash
   # Instalace závislostí (pokud ještě nejsou nainstalované)
   pip install -r requirements.txt
   
   # Generování dokumentu
   python scripts/generate_docx.py
   ```
3. **Nový dokument** najdete v `output/maturitni_otazky_ucetnictvi.docx`

**Automatické generování:** Po každém push do main větve s úpravami v `docs/src/otazky.md` se dokument automaticky vygeneruje pomocí GitHub Actions.
