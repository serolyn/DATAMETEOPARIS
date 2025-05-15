# Climat-Paris — Data Viz & Analyse météo (35 000 lignes)

> **TL;DR** : exploration Python + Pandas + Matplotlib d’un dump météo brut (2018-2024) sur Paris, nettoyage → corrélations → visualisations.  
> **Demo** : ▶️ `notebooks/00_overview.ipynb` (Binder badge plus bas).

---

## 0. Pourquoi ça existe ?

- **Objectif perso** : démontrer la chaîne complète _data-science “from scratch”_ (acquisition → cleaning → EDA → visu statique + interactive).
- **Question centrale** : _“Paris devient-il méditerranéen ou simplement chaotique ? Entre illusion régionale et réalité globale, comment comprendre le glissement du climat parisien dans un monde en désordre ?”_
- **Plus-value** : pipeline reproductible + figures prêtes pour un rapport académique.

---

## 1. Jeu de données

| Source | Période | Taille brute | Licence |
|--------|---------|--------------|---------|
| `data/meteo_paris_raw.csv` | 01-2018 ➜ 03-2024 | ~35 000 lignes | CC-BY 4.0 (Météo-France open-data) |

📄 **Dictionnaire de variables** : [`docs/variables.md`](docs/variables.md)

---

## 2. Stack & pré-requis

```bash
python 3.11
pip install -r requirements.txt   # pandas numpy matplotlib seaborn jupyter ...
