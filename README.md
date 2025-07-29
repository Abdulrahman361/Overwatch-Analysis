# Overwatch Match & Map Analysis

This project analyzes match and map-level statistics from the `match_map_stats.csv` dataset, focusing on team performance, map types (control vs. escort), win rates, and key gameplay metrics such as payload distances and time banks. Using **pandas**, **matplotlib**, and **seaborn**, the project provides visual and statistical insights that can help teams improve performance and league organizers adjust game rules.

---

## **Features**
- **Data Cleaning & Preparation**
  - Added `map_type` variable (control or escort) using control percentage data.
  - Converted time columns (`round_start_time`, `round_end_time`) to `datetime` format and extracted the match year.
  - Replaced irrelevant payload/time fields with `NaN` for control maps.

- **Team Performance**
  - Calculated **win rates** for all teams on control maps.
  - Created **rankings of teams** by 2022 control map win rate (1 = best, 20 = worst).
  - Analyzed trends over time (e.g., Shanghai Dragons’ win rate progression).

- **Toronto Defiant Insights**
  - Identified Toronto Defiant's **best and worst control maps** by win rate.
  - Evaluated opponent strengths using **mean rank comparisons**.
  - Suggested priority maps for 2023 training.

- **Draw Analysis (Escort Maps)**
  - Found that **46.54% of escort maps end in a draw**, far exceeding the 5% threshold.
  - Created a **bar plot of draws by map** to identify problematic maps.

- **Payload & Time-Bank Analysis**
  - Explored `attacker_time_banked` (when attackers win) and `attacker_payload_distance` (when attackers lose).
  - Visualized distributions using histograms and computed detailed summary statistics.

---

## **Technologies Used**
- **Python**: pandas, numpy, matplotlib, seaborn
- **Data Visualization**: Win rates, time-bank distributions, draw frequencies
- **Jupyter Notebook**: Interactive analysis and plots

---

## **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/overwatch-map-analysis.git
