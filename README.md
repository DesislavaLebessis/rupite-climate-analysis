# Climate Anomaly Analysis – Rupite, Bulgaria (1950–2024)

## Overview
Rupite is a small village in southwestern Bulgaria located at the foot of the extinct Kozhuh volcano. The area is known for its geothermal springs (74°C), diffuse CO₂ emissions from tectonic fault lines, and a unique Mediterranean-influenced microclimate.

This project investigates whether the geothermal activity of Rupite produces measurable climate anomalies compared to nearby cities over a period of 75 years (1950–2024).

---

## Research Question
> Does the geothermally active region of Rupite show consistent climate differences compared to the surrounding region – and do these differences remain stable over 75 years despite climate change?

---

## Key Findings

| Indicator | Rupite | Blagoevgrad (40km) | Sofia (130km) |
|---|---|---|---|
| Warming trend | +0.18°C/decade | +0.20°C/decade | +0.22°C/decade |
| Avg. frost days/year | 47 days | 71 days | 93 days |
| Spring onset | 24 February | 05 March | 17 March |
| Climate shift 1987 | +0.82°C | – | +0.90°C |

**Main conclusion:** Rupite shows consistently fewer frost days, earlier spring onset, and a slower warming trend than the surrounding region. The temperature difference between Rupite and Blagoevgrad (40km away, no geothermal activity) remained stable over 75 years (p=0.47), suggesting the geothermal effect is persistent but not amplified by climate change.

---

## Analyses

1. **Warming trend** – Linear regression of annual mean temperatures 1950–2024
2. **Climate shift 1987** – Comparison of mean temperatures before and after 1987
3. **Frost days** – Annual count of days with minimum temperature below 0°C
4. **Spring onset** – First day of year with mean temperature above 10°C
5. **Geothermal effect over time** – Temperature difference Rupite vs. Blagoevgrad over 75 years

---

## Data Source

- **Provider:** Open-Meteo Historical Weather API
- **Dataset:** ERA5 Reanalysis (ECMWF)
- **Resolution:** ~9km x 9km
- **Period:** 1950–2024
- **License:** CC BY 4.0
- **Note:** ERA5 reanalysis data are model-based estimates, not direct ground measurements. Results should be interpreted accordingly.

**Coordinates used:**
- Rupite: 41.47°N, 23.22°E
- Blagoevgrad: 42.01°N, 23.09°E
- Sofia: 42.70°N, 23.32°E

---

## Methods

- Python 3
- pandas – data processing
- scipy.stats – linear regression, significance testing
- matplotlib – visualization
- openmeteo-requests – data retrieval

---

## How to Run

1. Open the notebook in Google Colab
2. Run the first cell to install dependencies
3. Run all cells in order

```
!pip install openmeteo-requests requests-cache retry-requests
```

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com)

---

## Limitations

- Data based on ERA5 reanalysis, not direct station measurements
- No direct geothermal activity data included
- Causality between geothermal activity and climate anomaly not proven
- Further validation with real ground measurements recommended

---

## Author

**Desislava Lebessis**
Student of Economics, FernUniversität in Hagen, Germany
Citizen Scientist – SuperWASP / Zooniverse

GitHub: [DesislavaLebessis](https://github.com/DesislavaLebessis)
LinkedIn: [desislava-lebessis](https://www.linkedin.com/in/desislava-lebessis-57aa77b4)

---

## License

Code: MIT License
Data: CC BY 4.0 – Open-Meteo (open-meteo.com)
