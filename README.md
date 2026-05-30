# Sales Enablement ROI Analysis Dashboard

> **Interactive dashboard measuring the business impact of training programs on 9,247+ salespeople**

🚀 **[View Live Dashboard](https://srijanya-chetikaneni.github.io/sales-enablement-roi/)** | 📊 **[Technical Details](DATA_EXPLANATION_GUIDE.md)** | 💻 **[Code & Data](#repository-structure)**

---

## 🎯 The Business Problem

Every year, organizations invest millions in sales enablement programs—but struggle to answer one critical question:

**"Which programs actually drive revenue?"**

This dashboard solves that problem by measuring training impact at scale.

---

## 📈 Key Findings

**Training drives a permanent 26-point quota lift**
- Trained reps achieve **87% quota attainment**
- Untrained reps achieve **61% quota attainment**
- Lift persists from Month 4 onward (not temporary)

**Acceleration matters: 48 days faster to productivity**
- Trained reps reach productivity in **4.2 months**
- Untrained reps reach it in **5.8 months**
- Savings of 1.6 months per rep (high ROI on ramp)

**Sales Skills is the workhorse program**
- **$18.2M revenue impact** (highest)
- **15.2x ROI** (24-day payback)
- Highest completion rate: 89%

**Enterprise segment is the opportunity**
- Only **54% trained** (vs 78% in Mid-Market)
- Scaling from 54% → 75% trained = **$1.2M Year 1 upside**
- Clear scaling path identified

---

## 🏃 Quick Start

### View the Dashboard (No Installation)
1. Click the live link above
2. Select `index.html`
3. Click "Load Data from CSVs"
4. Explore 4 interactive charts

### Run Locally
```bash
# Install dependencies
pip install pandas numpy

# Generate data
python generate_enablement_data.py

# Start server
python -m http.server 8000

# Open browser
http://localhost:8000/index.html
```

---

## 📊 What You'll See

**4 Interactive Visualizations:**

1. **Quota Attainment Over Time** — Shows training impact ramping in Month 4, reaching 26-point lift by Month 6
2. **Ramp Time Distribution** — Compares trained vs untrained rep acceleration to productivity
3. **Program ROI by Type** — Ranks programs by revenue impact (Sales Skills > Product Knowledge > Tools > Soft Skills)
4. **Key Metrics Summary** — Critical business metrics at a glance

**All metrics are:**
- ✅ Derived from 110,940 data points (9,247 reps × 12 months)
- ✅ Segmented by business unit (Enterprise, Mid-Market, SMB)
- ✅ Methodologically sound (quasi-experimental design)
- ✅ Actionable (specific recommendations included)

---

## 💡 Business Insights

**What This Analysis Demonstrates**

This project shows how to translate operational data into business impact:

- **Causal Inference:** Designed quasi-experimental comparison (trained vs control) to isolate training effect from other variables
- **Segmentation:** Analyzed by business unit to surface Enterprise opportunity specifically
- **ROI Quantification:** Ranked programs by revenue impact AND efficiency (payback period)
- **Actionable Recommendations:** Moved from "enablement is good" to "scale Sales Skills to 85% and target Enterprise"

**Why This Matters for Your Organization**

Your Sales Enablement budget is 6-8 figures. This analysis:
- Justifies spend with data
- Identifies which programs deliver highest ROI
- Surfaces specific scaling opportunities
- Provides business case for continued investment

---

## 🛠 Technical Approach

**Methodology: Quasi-Experimental Design**

```
Treatment Group (Trained): 6,103 reps
Control Group (Untrained): 3,144 reps
Measurement Period: 12 months
Data Points: 110,940
```

**Key Variables Analyzed**
- Quota attainment (primary metric)
- Time to 50% quota (ramp productivity)
- Revenue per rep
- Segment-level variation
- Program completion & impact

**Why Synthetic Data?**

This is a proof-of-concept model using realistic parameters:
- Benchmarked to industry training effectiveness
- Validated against Gartner customer patterns
- Demonstrates analytical methodology, not predictions

With real data, this exact approach would add:
- Manager quality controls
- Territory potential segmentation
- Tenure and experience weighting
- Competitive intensity adjustments

---

## 📁 Repository Structure

```
sales-enablement-roi/
├── index.html                          # Interactive dashboard
├── generate_enablement_data.py         # Data generation script
├── README.md                           # This file
├── DATA_EXPLANATION_GUIDE.md           # Technical deep dive
├── enablement_data/
│   ├── reps.csv                       # 9,247 reps (master file)
│   ├── monthly_attainment.csv         # 110,940 rows (12 mo × reps)
│   └── programs.csv                   # 4 programs + ROI metrics

```

---

## 🎓 For Recruiters

**What This Project Shows**

✅ **Analytical Capability**
- Can frame business problems as data questions
- Understand causality vs correlation
- Design proper comparisons (trained vs control)

✅ **Technical Execution**
- Python data generation & ETL
- CSV handling and transformation
- Interactive visualization with real data

✅ **Business Communication**
- Translate metrics into insights
- Surface actionable recommendations
- Present complex analysis clearly

✅ **End-to-End Ownership**
- Problem definition through deployment
- Data generation to interactive dashboard
- GitHub to live URL (fully shipped)

---

## 📚 Learn More

**Want the full technical details?**
→ Read [DATA_EXPLANATION_GUIDE.md](DATA_EXPLANATION_GUIDE.md) for:
- Detailed methodology
- Statistical validation
- Segment-level analysis
- Interpretation guide for each chart

**Want to run this locally?**
→ See [Quick Start](#quick-start) above

**Want to build on this?**
→ All data generation code is open source
- Modify parameters (rep counts, training %)
- Adjust program impact assumptions
- Add new segments or metrics

---

## 🚀 Next Steps

1. **View the live dashboard** — [Click here](https://srijanya-chetikaneni.github.io/sales-enablement-roi/)
2. **Explore the data** — Download CSVs from the repo
3. **Read the methodology** — See [DATA_EXPLANATION_GUIDE.md](DATA_EXPLANATION_GUIDE.md)
4. **Run locally** — Follow [Quick Start](#quick-start)

---

## ❓ Questions?

**On the analysis?** Read [DATA_EXPLANATION_GUIDE.md](DATA_EXPLANATION_GUIDE.md)

**On the code?** All Python and HTML are documented. File issues or reach out.

**On the opportunity?** This analysis is designed to be a conversation starter for how data-driven insights can support Sales Enablement strategy and investment decisions.

---

## 👤 About

Built as a demonstration of analytical problem-solving in sales operations. This project shows how to measure what matters: not "did we train people?" but "did training drive quota?"

---

**Built with:** Python (Pandas, NumPy) | HTML/JavaScript | Chart.js | GitHub Pages

**Contact:** [LinkedIn](https://linkedin.com/in/srijanyachetikaneni) | [GitHub](https://github.com/srijanya-chetikaneni)

---

*This analysis uses synthetic data modeled on realistic sales enablement scenarios. Methodology and insights are applicable to real data.*
