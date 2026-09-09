Here is the complete, publication-ready **README.md** tailored specifically to the Udemy dataset, your KNIME node pipeline, and analytical findings, followed by simple instructions to publish it on GitHub.

---

### `README.md` File

```markdown
# 📚 Udemy Market Intelligence & Monetization Data App

An end-to-end data analytics pipeline and interactive decision-support application built with the **KNIME Analytics Platform**[cite: 4]. This project evaluates demand dynamics, monetization patterns, and content quality factors across 3,676+ online courses spanning four core subject domains[cite: 3, 4].

---

## 📌 Pipeline Architecture

The ETL workflow is designed to ingest multi-domain catalog records, engineer financial and temporal features, and bundle analytics into an interactive single-frame **Master Dashboard**[cite: 3, 4]:

```text
CSV Reader ──► Math Formula (Estimated Revenue) ──► String to Date&Time ──► Date&Time Part Extractor ──► Interactive Dashboard Component

```

### Transformation & Node Breakdown

* **Data Ingestion & Feature Engineering:** `CSV Reader` ➔ `Math Formula` ($\text{Estimated Revenue} = \text{Price} \times \text{Subscribers}$) ➔ `String to Date&Time` ➔ `Date&Time Part Extractor` (temporal trends 2011–2017).


* **Interactive Dashboard Component (`Udemy Analyt`):** Encapsulates `Nominal Row Filter Widgets`, `GroupBy`, `Table View`, `Histogram`, `Heatmap`, `Box Plot`, `Scatter Plot Matrix`, `Bar Charts`, `Line Plot`, and `Pie Chart`.



---

## 📊 Key Analytical Insights

### 1. Market Growth & Audience Concentration

* **The Historic Surge:** Course enrollments experienced exponential growth between 2011 and 2015, peaking above **3.5M annual subscribers** before stabilizing into a mature ecosystem.


* **The Beginner Magnet:** Over **85% of learners** congregate in "All Levels" (6.26M) and "Beginner Level" (4.14M) courses.


* **The Expert Paradox:** "Expert Level" courses account for less than 5% of enrollments (280k)—representing a niche volume target but an opportunity for high-ticket specialization.



### 2. Economics & The Pricing Paradox

* **Tech Dominance:** Web Development is the commercial engine of the catalog, generating approximately **$631M in estimated gross revenue**—more than 5x Business Finance ($124M), Graphic Design ($77M), and Music ($53M) combined.


* **Freemium Acquisition:** Free ($0) courses capture substantial top-of-funnel traffic (spiking up to 268k subscribers per course).


* **Premium Price Ceiling:** Courses at the top tier ($200) maintain strong subscriber volumes, disproving the assumption that demand drops sharply at higher price points for technical subjects.



### 3. Course Quality & Engagement Moats

* **Duration Norms vs. Outliers:** Median course duration sits between **2 and 5 hours** across all difficulty levels to reduce cognitive fatigue, while flagship outlier courses scale from **30 to 80+ hours** to build durable competitive moats.


* **Rating Consistency:** Satisfaction scores are positively skewed, concentrating between **0.70 and 0.95+** across domains and course levels.


* **The Review Flywheel:** Scatter plot matrix analysis confirms that review velocity is the single strongest statistical driver of compounding subscriber acquisition.



---

## 📈 Core Market Benchmarks

| Metric | Benchmark | Context |
| --- | --- | --- |
| **Catalog Depth** | **3,676 Courses** | Evaluated across Business, Web Dev, Graphic Design, and Music

 |
| **Peak Domain Revenue** | **~$631 Million** | Total estimated revenue captured by Web Development

 |
| **Mass Market Demand** | **>85%** | Share of subscribers enrolled in Beginner and All-Level courses

 |
| **Median Duration** | **2 – 5 Hours** | Standard course length balancing completion with depth

 |

---

## 📁 Repository Contents

* `Udemy_Courses_Data_App.knwf`: Exported, portable KNIME workflow package configured with workflow-relative paths.


* `data/`: Clean CSV datasets divided by discipline (`business-courses.csv`, `design-courses.csv`, `music-courses.csv`, `web-development.csv`).


* `Udemy_Analytics_Master_Deck.pdf`: Executive presentation detailing findings, market strategies, and visualization components.



---

## 🚀 How to Run the Project

1. Install [KNIME Analytics Platform](https://www.knime.com/downloads).


2. Download or clone this repository:
```bash
git clone [https://github.com/jilinsebastian123/udemy-market-intelligence-data-app.git](https://github.com/jilinsebastian123/udemy-market-intelligence-data-app.git)

```


3. In KNIME, navigate to **File > Import KNIME Workflow...** and select the `.knwf` file.


4. Run the workflow, right-click the wrapped composite component (`Udemy Analyt`), and select **Interactive View** to explore the dashboard.



```

---

### Step-by-Step: Adding This to GitHub

1. **Export the Workflow:** In KNIME, right-click your `Udemy_Courses_Data_App` workflow, click **Export KNIME Workflow...**, check **Reset workflow before export**, and save it as `Udemy_Courses_Data_App.knwf`[cite: 3].
2. **Save Slides as PDF:** Open `Udemy Analytics Master Dataapp.pptx` in PowerPoint, click **File > Save As / Export > PDF**, and name it `Udemy_Analytics_Master_Deck.pdf`[cite: 4].
3. **Create the New Repository:**
   * Go to [github.com/new](https://github.com/new).
   * **Repository Name:** `udemy-market-intelligence-data-app`
   * **Visibility:** Public
   * Leave README, .gitignore, and license **unchecked**, then click **Create repository**.
4. **Upload Files:**
   * Click **"uploading an existing file"**.
   * Drag in `Udemy_Courses_Data_App.knwf`, `Udemy_Analytics_Master_Deck.pdf`, and your CSV files from the `data/` folder[cite: 3, 4].
   * Click **Commit changes**.
5. **Create README.md:**
   * Click **Add file > Create new file**, name it `README.md`, paste the text above, and commit changes.
6. **Pin to Profile:**
   * Navigate to your main GitHub profile, click **Customize your pins**, check `udemy-market-intelligence-data-app`, and save.

```
