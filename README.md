# Maturitní otázky – Účetnictví (ČR)

## Kde najdu hotový dokument? / Where can I find the done document?

**✅ Dokument je připraven!** Najdete ho v adresáři `output/maturitni_otazky_ucetnictvi.docx`

**✅ The document is ready!** You can find it in the `output/maturitni_otazky_ucetnictvi.docx` directory

---

## Plánovaná struktura repozitáře / Planned Repository Structure

Po dokončení bude repozitář obsahovat:

- **`output/`** – Zde bude finální Word dokument (.docx) s 22 otázkami
  - **This is where the final document will be located**
- **`docs/src/otazky.md`** – Zdrojový obsah v Markdownu (22 kapitol)
- **`scripts/generate_docx.py`** – Python skript pro generování .docx
- **`.github/workflows/`** – GitHub Actions workflow pro automatické sestavení

---

## Co je třeba udělat / What needs to be done

1. **Vyplnit obsah otázek** v souboru `docs/src/otazky.md`
   - 22 kapitol, každá cca 1× A4
   
2. **Vytvořit Python skript** `scripts/generate_docx.py`
   - Použít knihovnu `python-docx`
   - Formát: Times New Roman 12, řádkování 1.5, okraje 2.5 cm
   - Titulní strana, obsah, kapitoly 1–22 (každá na nové stránce)
   - Číslování stránek od 1. kapitoly
   
3. **Nastavit GitHub Actions workflow**
   - Automatické generování .docx při změnách
   - Uložení výstupu do `output/`

4. **Spustit generování**
   - Hotový dokument se objeví v adresáři `output/`

---

## Jak používat / How to use

Po dokončení nastavení:

```bash
# Instalace závislostí
pip install python-docx

# Generování dokumentu
python scripts/generate_docx.py

# Výstup bude v:
# output/maturitni_otazky_ucetnictvi.docx
```

---

## Formát dokumentu / Document Format

- **Font:** Times New Roman 12
- **Řádkování / Line spacing:** 1.5
- **Okraje / Margins:** 2.5 cm
- **Struktura / Structure:**
  - Titulní strana
  - Obsah
  - Kapitoly 1–22 (každá na nové stránce)
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
