# Pokémon PCA: Multi-Dimensional Stat Analysis & Visualization

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-orange.svg)](https://scikit-learn.org/)
[![Plotly](https://img.shields.io/badge/Plotly-Interactive-brightgreen.svg)](https://plotly.com/)

An advanced analytical study of Pokémon combat statistics using **Principal Component Analysis (PCA)**. This project transforms the traditional 6-dimensional stat space (HP, Attack, Defense, Sp. Atk, Sp. Def, Speed) into a high-impact 2D landscape, revealing latent patterns in Pokémon roles, power scaling, and generation-over-generation power creep.

---

## 🚀 Key Features

- **PCA Dimensionality Reduction**: Compressed 6 combat stats into 2 Principal Components, capturing over **63% of the total variance**.
- **Interactive Global Map**: A full-scale Plotly visualization of 800+ Pokémon, filterable by type and generation.
- **Power Creep Analysis**: Quantitative comparison of Base Forms vs. Special Forms (Megas, Primals) across generations.
- **Type Centroid Mapping**: Identified the "center of mass" for each Pokémon type within the PCA space to visualize type-based niches (e.g., the "Tankiness" of Steel vs. the "Speed" of Electric).
- **Special Form Identification**: Automated feature engineering to distinguish between standard Pokémon and specialized forms.

---

## 📊 Methodology & Interpretation

### Principal Component Analysis
The analysis reveals two distinct latent dimensions that define a Pokémon's competitive identity:

1.  **PC1 (45.7% Variance) — "General Power & Endurance"**: 
    - Strongly correlated with high HP, Defenses, and Attacks.
    - Represents the overall "Magnitude" of a Pokémon's stat pool.
2.  **PC2 (18.2% Variance) — "Specialization vs. Technicality"**:
    - High PC2: Fast, glass-cannon specialized attackers (Speed/Sp. Atk).
    - Low PC2: Slow, bulky physical walls (Defense/HP).

### Visualizations Included
- **Interactive PCA Scatters**: Detailed hover data including Name, Type, and PC coordinates.
- **Type-Density Facet Grids**: Comparison of how different types occupy the stat landscape.
- **Power Trend Plots**: Line and box plots showing the rising stat floor through different generations.

---

## 🛠️ Tech Stack

- **Data Manipulation**: `Pandas`, `NumPy`
- **Machine Learning**: `Scikit-Learn` (StandardScaler, PCA)
- **Static Visualization**: `Seaborn`, `Matplotlib`
- **Interactive Visualization**: `Plotly Express`

---

## 📂 Dataset

The data is based on the comprehensive Pokémon dataset provided by [lgreski/pokemonData](https://github.com/lgreski/pokemonData.git).

---

## 📥 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/GiaHuy/PokemonPCA.git
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn plotly
   ```
3. Run the notebook:
   ```bash
   jupyter notebook pokemon_pca.ipynb
   ```

---

## 📝 License

This project is intended for educational and analytical purposes. Pokémon and its character names are intellectual property of Nintendo, Game Freak, and Creatures.