# 🏙️ Lombardia Vivibile

**Data Management** | Università degli Studi di Milano-Bicocca | A.A. 2025/2026  
*Alberto Cera, Fabio Focchi*

## 📌 Overview
Construction of a composite liveability index (0–100) for five major 
Lombard cities — Milan, Brescia, Bergamo, Monza, and Como — by 
integrating heterogeneous data from publicly available sources through 
a complete data management pipeline.

## 🔍 Research Questions
- Which Lombard city ranks highest on a multidimensional liveability index?
- Which dimensions contribute most to liveability?
- Are urban parks located in areas with acceptable air quality?
- Are the datasets reliable enough for quantitative comparison?

## 🗄️ Data Sources
| Source | Technique | Data |
|--------|-----------|------|
| OpenStreetMap (Overpass API) | REST API | Green areas, cultural POIs, bus stops |
| ARPA Lombardia | CSV Download | NO2, Ozone, Benzene measurements |
| ISTAT | ZIP Download | Population by age group and gender |

## 🛠️ Tech Stack
- **Python 3.11** — JupyterLab
- **MongoDB 5.0** — NoSQL storage
- **pymongo, pandas, numpy, matplotlib**
- **Docker + Azure Lab Services**

## 📊 Results
| Rank | City | Index |
|------|------|-------|
| 1 | Bergamo | 70.5 |
| 2 | Milan | 67.5 |
| 3 | Monza | 66.6 |
| 4 | Brescia | 48.4 |
| 5 | Como | 26.9 |

## 📁 Structure
```
├── 01_acquisizione_osm.ipynb
├── 02_acquisizione_arpa.ipynb
├── 03_acquisizione_istat.ipynb
├── 04_integrazione.ipynb
├── 05_profiling.ipynb
├── 06_analisi_esplorativa.ipynb
└── 07_arricchimento_spaziale.ipynb
```
