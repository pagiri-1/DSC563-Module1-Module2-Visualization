# DSC 563 – Module 1 and Module 2 Visualization Project

## Project Overview
This project analyzes simulated community workshop attendance and utilization data using Google Colab (Python) and Tableau.

**Research Question:** How does workshop attendance vary across neighborhoods, and how do utilization rates compare?

**Target Audience:** Community workshop coordinators and program managers.

## Data Source
The workshop dataset is simulated for educational purposes and covers June–November 2026. Attendance visits represent seat visits rather than unique participants. Workshop capacity varies by neighborhood and month.

## Project Files
- `tableau_workshops_tidy.csv` – Prepared workshop dataset.
- `m01_after_chart.png` – Module 1 Python visualization.
- `m01_claim_check.csv` – Checked Python values.
- `module_2_file_guide.txt` – Guide to the exported files.
- Module 1 `.ipynb` notebook – Python analysis and Module 2 verification.
- `Module2_Tableau_Verification.png` – Tableau verification screenshot.

## Module 1: Python Analysis
The Python notebook creates and verifies a November 2026 workshop attendance chart.

## Module 2: Python vs. Tableau Verification

**Selected Month:** November 2026

**Measure:** Total attendance visits

**Aggregation:** SUM of attendance visits by neighborhood

| Neighborhood | Python | Tableau | Difference |
|---|---:|---:|---:|
| East | 94 | 94 | 0 |
| West | 90 | 90 | 0 |
| North | 90 | 90 | 0 |
| South | 82 | 82 | 0 |

All four Tableau values match the checked Python values.

## Graduate-Level Utilization Comparison

Two utilization measures were compared across the available months:

1. Average monthly utilization: the arithmetic mean of observed monthly utilization percentages.
2. Capacity-weighted utilization: total observed attendance divided by total corresponding capacity, multiplied by 100.

| Neighborhood | Average Monthly | Capacity-Weighted | Observed Months |
|---|---:|---:|---:|
| East | 73.4% | 73.57% | 5 of 6 |
| North | 73.1% | 73.17% | 6 of 6 |
| South | 79.9% | 80.00% | 6 of 6 |
| West | 59.2% | 59.36% | 6 of 6 |

The weighted measure accounts for differences in workshop capacity, while the average monthly measure gives each observed month equal weight.

East has missing attendance for one month. This comparison excludes that missing observation rather than treating it as zero attendance. Consequently, East's utilization is based on fewer observed months and should be interpreted cautiously.

**Interpretation:** South has the highest utilization under both methods. The methods produce slightly different percentages but do not change the neighborhood ranking.

**Limitation:** The dataset is simulated, and missing observations may affect the interpretation of utilization.

## Reproducing the Analysis
1. Open the personal Module 1 notebook in Google Colab.
2. Run the notebook cells to reproduce the Python chart and checked values.
3. Open the Tableau workbook or Tableau Public view.
4. Select November 2026, neighborhood, and SUM of attendance visits.
5. Compare the four neighborhood values with `m01_claim_check.csv`.
6. Review the Tableau utilization and observed-month coverage worksheets.

## Project Links
- **Google Colab:** [(https://colab.research.google.com/drive/1b7Y6VcDmIw2eH1Co0IWz2pPQuRZW_fs5?usp=sharing)
- **Tableau Public:** https://public.tableau.com/app/profile/pasmina.giri/viz/DSC63_MODULE2_Tabeau/November2026AttendenceVerification5?publish=yes

## Data Attribution and Use
This project uses simulated educational workshop data. Original source attribution and any reuse restrictions should follow the course-provided dataset documentation.
