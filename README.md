
---

# 📁 3. Virat Kohli All-Format Statistics (Power BI & Excel)

```markdown
# 🏏 Virat Kohli Career Performance Analytics — Power BI & Excel

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=power-bi&logoColor=black)
![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Sports Analytics](https://img.shields.io/badge/Sports_Analytics-008080?style=for-the-badge)
![DAX](https://img.shields.io/badge/DAX_Measures-00758F?style=for-the-badge)

## 📌 Project Overview
An interactive **Sports Analytics Dashboard** built using **Microsoft Power BI** and **Excel** to analyze the international batting career of cricket icon **Virat Kohli** across all three major formats: **Test, ODI, and T20I**.

This project models historical match statistics to assess batting consistency, strike rate dynamics, boundary percentages, and year-by-year performance evolution.

---

## 🎯 Analytical Metrics Explored
* **Format-Wise Comparison**: Comprehensive comparison between Test, ODI, and T20 International appearances.
* **Volume Metrics**: Total Innings, Runs Scored, Balls Faced, and Outs.
* **Efficiency & Scoring Rate**:
  * **Batting Average (Avg)**: Runs scored per dismissal.
  * **Strike Rate (SR)**: Scoring speed per 100 deliveries.
* **Boundary Analysis**: Total 4s and 6s scored, boundary run contribution, and **Dot Ball %**.
* **High Scores & Milestones**: Tracking peak scores (HS) and century conversion consistency.
* **Year-by-Year Career Trajectory**: Evolution of Kohli's peak run-scoring calendar years.

---

## 🗄️ Dataset Schema (`Virat Kohli Statistics.xlsx`)
The dataset includes granular career statistics broken down across multiple dimensions:

| Field Name | Description |
|---|---|
| `Format` | Match format (`Test`, `ODI`, `T20i`) |
| `Year` | Calendar year of competition |
| `Innings` | Total innings batted |
| `Runs` | Cumulative runs scored |
| `Balls` | Total deliveries faced |
| `Outs` | Total dismissals |
| `Avg` | Calculated Batting Average (`Runs / Outs`) |
| `SR` | Strike Rate (`(Runs / Balls) * 100`) |
| `HS` | Highest score achieved in the period |
| `4s` | Number of boundaries (fours) hit |
| `6s` | Number of maximums (sixes) hit |
| `Dot %` | Percentage of dot balls faced |

---

## 🛠️ Power BI Features & DAX Implementations
* **Interactive Slicers**: Seamlessly toggle between Test, ODI, and T20I formats or select specific year ranges.
* **Custom DAX Measures**:
  * `Batting Average = DIVIDE(SUM('Overall'[Runs]), SUM('Overall'[Outs]), 0)`
  * `Strike Rate = DIVIDE(SUM('Overall'[Runs]), SUM('Overall'[Balls]), 0) * 100`
  * `Boundary Contribution % = DIVIDE((SUM('Overall'[4s])*4 + SUM('Overall'[6s])*6), SUM('Overall'[Runs]), 0)`
* **Dynamic KPI Cards**: Instant summary of total career runs, centuries, global average, and overall strike rate.
* **Custom Cricket Visual Theme**: High-contrast, clean sports visualization theme designed for clarity and aesthetic appeal.

---

## 💡 Key Analytical Takeaways
1. **ODI Masterclass**: Kohli maintains an astronomical batting average exceeding 55+ in ODIs with an elite chase conversion rate.
2. **Strike Rate Evolution**: Demonstrates a calculated acceleration curve in T20Is without sacrificing wicket preservation.
3. **Peak Dominance Era (2016–2019)**: Visualizes the unprecedented peak across all formats where his calendar-year averages consistently crossed 60+.
4. **Boundary vs. Strike Rotation**: Proves that despite hitting fewer high-risk sixes than pure power-hitters, low dot-ball percentages and running between wickets maintain a world-class strike rate.

---

## 🖥️ How to Run
1. Ensure you have **Microsoft Power BI Desktop** installed.
2. Clone this repository:
   ```bash
   git clone https://github.com/Salehaparween/Virat-Kohli-Statistics.git
