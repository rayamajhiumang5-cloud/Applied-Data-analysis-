# Applied-Data-analysis- In class Lab2 Documentation 

```markdown
# The Illusion of Growth & the Composition Effect
**Deflating History with FRED**

## Objective
This project investigates long-run U.S. wage growth by combining live macroeconomic data from the Federal Reserve Economic Data (FRED) API with inflation adjustments and labor-market controls. The primary goal is to test whether observed wage growth reflects genuine improvements in workers’ purchasing power—or whether it is distorted by inflation and statistical composition effects.

By constructing a reproducible Python data pipeline, this lab exposes the difference between **nominal wage growth**, **real wage stagnation**, and **composition-driven statistical illusions**.

---

## Methodology

### Data Ingestion (FRED API)
- Pulled nominal wage data (**AHETPI – Average Hourly Earnings**) directly from FRED using `fredapi`.
- Retrieved Consumer Price Index (CPI) data to deflate nominal wages and compute real wages.
- Fetched the **Employment Cost Index (ECI)** to control for changes in workforce composition.

### Analytical Pipeline
1. Converted nominal wages into real wages to remove inflationary distortions.
2. Visualized long-run trends (1960s–present) to evaluate real purchasing power.
3. Identified a sharp wage spike in 2020 during the COVID-19 recession.
4. Applied the Employment Cost Index as a fixed-composition benchmark to isolate and correct for the **composition effect**—holding job mix constant across time.

### Tools & Stack
- Python
- `fredapi` (live macroeconomic data ingestion)
- `pandas` (time-series processing and transformations)
- `matplotlib` (economic data visualization)

---

## Key Findings: The Pandemic Paradox
- **The Money Illusion:** While nominal wages have risen steadily for decades, real wages—after inflation adjustment—have remained largely flat, revealing persistent stagnation in purchasing power.
- **The Pandemic Spike (2020):** Standard wage measures show a sudden wage “boom” during the COVID-19 recession.
- **Composition Effect Exposed:** Using the Employment Cost Index demonstrates that this spike was **not** driven by rising labor demand or productivity gains. Instead, it resulted from disproportionate job losses among low-wage workers, mechanically raising the average wage.
- **Corrected Interpretation:** When workforce composition is held constant, wage growth remains stable and gradual—confirming that the 2020 surge was a statistical artifact, not a structural improvement in worker earnings.

---

##  Conclusion
This lab demonstrates how misleading aggregate statistics can be without proper economic controls. By integrating inflation adjustments and fixed-composition indices, the project highlights the importance of methodological rigor when interpreting labor market data—especially during economic shocks.
```

If you want, I can also **add badges and a table of contents** so it looks even more like a polished GitHub project README.

Do you want me to do that next?
