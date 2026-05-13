# Visualisation in Data Science — Group 4
## Air Quality in Madrid (2001–2017)

This project analyses hourly air pollution measurements from 24 monitoring 
stations across Madrid between 2001 and 2017. It was developed as part of 
the VDS2526 course at Hasselt University.

The analysis focuses on five key pollutants: NO₂, O₃, PM10, SO₂ and CO. 
The central finding is that while most pollutants have declined over the 
16-year period, ozone (O₃) has been quietly rising — and this project 
shows where and when it peaks.

---

## Requirements

- Python 3.12
- pandas 3.0.1
- plotly 6.6.0
- JupyterLab 4.5.6

Install dependencies using conda:

```bash
conda create -n vid python=3.12
conda activate vid
pip install pandas plotly jupyterlab kaleido
```

---

## Data

The data is not included in this repository due to file size.

To reproduce the visualisations, download the dataset (stations.csv and 
all files from the csvs_per_year folder) from 
https://www.kaggle.com/datasets/decide-soluciones/air-quality-madrid 
and place them in the following location:

data/VDS2526_Madrid/

---

## How to run

1. Clone the repository:
```bash
git clone https://github.com/nkemahjunior/visualization-in-data-science-implementation.git
cd visualization-in-data-science-implementation
```

2. Activate your environment:
```bash
conda activate vid
```

3. Launch JupyterLab:
```bash
jupyter lab
```

4. Open `notebooks/madrid_air_quality.ipynb` and run all cells from top 
to bottom.

---

## Visualisations

**Design 1 — Pollution Trends (2001–2017)**
A line chart showing the percentage change in concentration of five key 
pollutants relative to their 2001 baseline. O₃ is highlighted in red as 
the only pollutant trending upward over the period.

**Design 2 — O₃ Levels by Station (2017)**
A horizontal bar chart ranking all Madrid monitoring stations by their 
average O₃ concentration in 2017. A WHO guideline reference line is shown 
at 60 µg/m³.

**Design 3 — O₃ Peak Patterns by Hour and Month (2001–2017)**
A heatmap showing average O₃ concentration across all combinations of 
month and hour of day, revealing that peak O₃ occurs during summer 
afternoons.

---

## Authors

- Junior Nkemah Kaving
- Naveed Akhtar
- Nahom Melese Geremw
- Rexford Holland
- Gilbert Ihame