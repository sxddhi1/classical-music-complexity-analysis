# Musical Complexity Analysis Using Business Intelligence

**A Power BI dashboard analyzing structural complexity in classical MIDI compositions.**

> Built as part of a CSE_4018 Business Intelligence & Analysis class assessment.

---

## Project Overview

Music composition contains many structural elements that influence how complex a piece sounds — rhythm, harmony, melody variation, and note density. But how do you *measure* that complexity quantitatively?

This project uses Power BI to analyze a dataset of classical MIDI compositions and explore which musical features drive complexity, how those features relate to each other, and how complexity is distributed across compositions.

MIDI (Musical Instrument Digital Interface) compositions are digital music files that store notes, timing, and instrument data rather than actual audio. Unlike MP3s, they capture the *structure* of music — which makes them ideal for analyzing musical features like note density, key changes, and melody patterns programmatically.

---

## Goals

| Goal | Description |
|------|-------------|
| **Goal 1** | Identify which musical features contribute most to complexity |
| **Goal 2** | Understand how complexity changes with musical characteristics |
| **Goal 3** | Visualize the distribution of complexity across compositions |

---

## Dataset Description

The dataset consists of classical MIDI compositions extracted from musical archives. Each row represents a unique composition with the following attributes:

| Column | Description |
|--------|-------------|
| `Index` | Overall musical complexity score (target variable) |
| `NPS` | Notes Per Second — measures rhythmic density |
| `Entropy` | Measures unpredictability in the melody |
| `Polyphony` | Number of simultaneous notes played |
| `Chromaticism` | Frequency of semitone transitions |
| `Key` | Musical key of the composition |
| `Changes` | Number of key changes in the composition |
| `File` | Unique identifier for each composition |

---

## Dashboard


>  **open `dashboard_music.pbix` in Power BI Desktop to view the full interactive dashboard.**

The dashboard is divided into **3 sections**:

### Section 1 — KPI Metrics
Summary statistics giving a quick overview of the dataset:
- **Average Complexity Score: 58.97** (moderate complexity overall)
- **Average Musical Entropy: 4.56**
- **Average Chromaticism: 0.23**
- **Average Key Changes: 4.50**
- **Average Notes Per Second: 2.37**

### Section 2 — Relationship Analysis
Charts exploring how individual features influence complexity:
- **Key Changes vs Musical Complexity** — complexity rises steadily as key changes increase
- **Rhythmic Density vs Musical Complexity** — higher NPS corresponds with higher complexity
- **Melodic Entropy vs Complexity** — higher entropy correlates with higher complexity

### Section 3 — Distribution & Dataset Characteristics
- **Distribution of Musical Complexity** — histogram showing spread of complexity scores across all compositions
- **Distribution of Key Changes** — majority of compositions have few key changes
- **Most Common Musical Keys** — donut chart; C major is the most frequent key (102 compositions, ~7.99%)
- **Feature Contribution Chart** — compares average NPS, Entropy, Key Changes, and Chromaticism side by side

---

## Visualisation Techniques Used

- **KPI Cards** — for at-a-glance summary metrics
- **Histograms** — to analyze distribution of complexity and key changes
- **Bar Charts** — to show feature-complexity relationships
- **Feature Contribution Chart** — multi-metric clustered bar chart
- **Donut Chart** — to show proportion of compositions by musical key

---

## Key Insights

1. The average musical complexity score is **58.97**, indicating moderate complexity across the dataset.
2. **More key changes = higher complexity.** Compositions with more harmonic movement are measurably more complex.
3. **Higher entropy → higher complexity.** Unpredictable melodies are a strong indicator of complex compositions.
4. **Rhythmic density matters.** Compositions with more notes per second tend to score higher on complexity.
5. **C major dominates** the dataset, appearing in ~8% of all compositions, followed by C# major and B minor.
6. Musical complexity is driven by **multiple features together**, not any single attribute in isolation.

---

## Tools Used

- **Power BI Desktop** — dashboard creation and data visualization
- **Microsoft Excel** — data preparation (`Master_Complexity_Report.xlsx`)


---

## Files in This Repository

| File | Description |
|------|-------------|
| `dashboard_music.pbix` | Main Power BI dashboard file |
| `Master_Complexity_Report.xlsx` | Source dataset |
| `README.md` | This file |

---

## How to Open the Dashboard

1. Download and install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Clone or download this repository
3. Open `dashboard_music.pbix` in Power BI Desktop
4. Explore the interactive dashboard — use filters and slicers to drill down into the data

---

## Author

**Siddhi Gupta** 
