
# 🏀 NBA DraftKings Lineup Optimization – Feb 22, 2024

This project explores a real-world sports analytics problem—optimizing a fantasy basketball lineup for DraftKings Daily Fantasy Sports (DFS). Using actual NBA data from February 22, 2024, and historical season statistics, I used Python and optimization modeling techniques to construct the most effective lineup possible within given constraints.

## 🎯 Project Overview

Imagine competing in a DraftKings NBA DFS contest with 12 real NBA games played on Feb 22, 2024. The objective is to select an **8-player lineup** that maximizes total fantasy points under a **$50,000 salary cap** and position-specific constraints.

I built **two optimization models**:
- 📊 **Model 1 – Historical-Based Lineup**: Uses player performance trends, opponent strength, and home/away advantages to build a predictive strategy.
- 🔍 **Model 2 – Actual-Based Lineup**: Uses actual game-day performance as a benchmark or “cheat code” for comparison.

## ⚙️ Constraints

The lineup must meet these DraftKings rules:
- Max **salary cap**: $50,000
- Must include **8 players**:
  - 1 PG, 1 SG, 1 SF, 1 PF, 1 C
  - 1 G (PG/SG), 1 F (SF/PF), 1 UTIL (any position)
- Must include players from **at least two different games**

## 🧠 Strategy Highlights

Instead of simply selecting players based on average fantasy points per game, this project explores deeper insights such as:
- Player rest days and their impact on performance
- Matchups against strong or weak defenses
- Synergistic picks (e.g., PG + SG from the same team = points + assists)
- Home-court advantage

## 🛠️ Tools & Libraries

- **Python**
- `pandas` – data wrangling
- `pyomo` – optimization modeling
- `matplotlib` / `seaborn` – visualizations
- `openpyxl` – Excel file handling
- `scikit-learn` – optional modeling components (e.g., regression)
  
## 📁 Project Structure

**NBA_DFS_Optimization**



-`FinalProjectNBA.ipynb`   -       **Main Jupyter notebook with data analysis and optimization logic**

- `NBAProject1.xlsx`       -       **Dataset containing historical and actual NBA player stats**
  
-`DKSalaries.csv`          -       **DraftKings salary, position, and average PPG info**

-`PlayerStats.csv `        -       **Full-season player statistics through Feb 21, 2024**

- `game_data/`             -        **Folder with individual game box scores from Feb 22, 2024**
  
- `FinalProjectNBA.html`   -      **Optional HTML rendering of the notebook for quick viewing**
  
  - `README.md`            -         **Project overview and instructions**

> *Note: Additional files used in the original assignment (e.g., DKSalaries.csv, PlayerStats.csv, and individual game box scores) were consolidated into `NBAProject1.xlsx`.*

## 📈 Key Outcomes

- Generated an optimal historical lineup strategy that reflects deeper domain insights.
- Benchmarked this model against the actual performance data to evaluate accuracy.
- Demonstrated how mathematical modeling can support real-world decision-making in fantasy sports.

## ✅ How to Run

1. Clone the repo:
```bash
git clone https://github.com/yourusername/NBA_DFS_Optimization.git
cd NBA_DFS_Optimization
