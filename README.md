# Funding Futures: Exploring K-12 Education Finance Equity with R

A guided data science lesson plan that uses real U.S. school district finance data to explore the relationship between funding and educational equity.

## 📖 Overview

**Funding Futures** is an interactive lesson plan designed for high school students, college undergraduates, and educators interested in understanding education policy through data. Using R and real federal data, students investigate a central question:

> *Does where you grow up — and how much money your school district has — shape your path to college and career?*

By connecting school finance data to student outcomes, this lesson develops critical thinking about educational equity, data interpretation, and the impact of resource distribution.

## 🎯 Whats Covered

- **Data Wrangling**: Clean and explore large federal datasets using R and the `tidyverse`
- **Equity Analysis**: Visualize relationships between poverty rates and school funding across districts
- **Policy & Data**: Connect abstract finance metrics to real student outcomes using the California C2C Student Pathways Dashboard
- **Data Literacy**: Understand data suppression protocols, their purpose, and their limitations
- **Research Design**: Formulate data-driven questions about education equity and design analyses to answer them

## 📈 Learning Outcomes

Upon completion, students will be able to:

✅ Load and explore multi-source federal and state education data  
✅ Create publication-quality visualizations of equity disparities  
✅ Interpret correlation between funding and poverty (and understand causation limits)  
✅ Navigate privacy-preserving data practices and understand their limits  
✅ Connect data findings to real-world policy questions  
✅ Formulate defensible research questions using education data  

## 🎓 Alignment

This lesson aligns with:
- **K-12 Data Literacy Standards**: Reading, creating, and critically interpreting data visualizations
- **College & Career Readiness**: Introduction to policy analysis and empirical research methods
- **California Social Science Standards**: Education, equity, policy, and civic participation

## 📝 Notes for Educators

- **Scaffolding**: The lesson is heavily scaffolded; reflection questions guide thinking. Encourage students to answer in their own words before class discussion.
- **Extensions**: The "Going Further" section includes advanced analyses (full dataset, wage trends, regional comparisons). Adapt based on student interest and time.
- **Discussion**: Use Checkpoint questions as springboards for classroom discussions about fairness, representation, and data interpretation.
- **Accessibility**: All visualizations use accessible color palettes (colorblind-friendly). Alt-text recommendations are in the code comments.

---

## 🏗️ Lesson Structure

The notebook is organized into three scaffolded parts, each with checkpoint reflection questions:

### **Part A: Getting Started with `edfinr`**
- Introduction to the edfinr R package and combined federal dataset
- Loading California K-12 school finance data (2011–2022)
- Exploring key variables: enrollment, revenue sources, demographics, poverty rates

### **Part B: Equity Visualizations**
- Core question: Does poverty predict funding disparities?
- Scatter plots and trend analysis of poverty vs. per-pupil revenue
- Revenue breakdown by source (local, state, federal)
- Multi-year trends and state-to-state comparisons

### **Part C: Connecting to Student Outcomes**
- Bridge from finance inputs to student outcomes
- Introduction to the California C2C Student Pathways Dashboard
- Understanding data suppression protocols and their equity implications
- Integration challenge: selecting districts to compare funding to real outcomes

### **Exit Ticket**
Four reflective questions requiring students to:
1. Formulate an original research question
2. Identify variables and data sources
3. Explain how data suppression affects analysis
4. Reflect on which communities are represented in data

## 📊 Data Sources

This lesson uses publicly available federal and California state data:

| Source | Coverage | Variables |
|--------|----------|-----------|
| **NCES F-33 Survey** | All U.S. school districts, 2011–22 | Revenue (local/state/federal), expenditures, district characteristics |
| **Census SAIPE** | School district level | Student poverty rates |
| **ACS 5-Year Estimates** | Community level | Demographics: income, educational attainment |
| **C2C Student Pathways Dashboard** | California school districts | Graduation rates, college enrollment, post-secondary outcomes |
| **C2C Wage Data** | California post-secondary students | Starting wages by award type (2018–2022) |

All data is aggregated and publicly available; no student-level identifiable data is used.

--- 

## 🚀 Getting Started

### Prerequisites
- **R** (version 4.0 or higher recommended)
- **RStudio** or similar R IDE
- Basic familiarity with R (data frames, tidyverse optional but helpful)

### Installation & Setup

1. **Clone or download this repository**
   ```bash
   git clone <repo-url>
   cd "CA Cradle-2-Career Lesson Challenge"
   ```

2. **Install required R packages**
   Open R and run:
   ```r
   install.packages(c("edfinr", "tidyverse", "scales", "ggrepel", "skimr", "janitor"))
   ```

3. **Open the lesson notebook**
   - Open `Funding_Futures_Notebook.Rmd` in RStudio
   - Run the setup chunk first to load all libraries

### Using This Lesson

**For Instructors:**
- The notebook includes scaffolded learning sections with "Checkpoint" reflection questions
- Each checkpoint is a code chunk where students write answers as comments
- The exit ticket (4 short-answer questions) serves as a final assessment
- Estimated time: 2–3 hours (can be split across multiple sessions)
- Modifications: Adjust state comparisons, extend analysis, or focus on specific regions

**For Self-Directed Learners:**
- Read each section carefully, run the code, and complete the reflection questions
- The "Going Further" section (optional extensions) provides deeper dives into the data
- Use the C2C Dashboard resources and external links provided in the notebook

## 💡 Key Concepts Covered

### Education Funding Equity
- **Revenue regressive**: Many U.S. districts rely heavily on local property taxes, creating inequities (wealthy areas → more funding)
- **Federal Title I**: Targeted funding for high-poverty districts; question: does it adequately compensate?
- **State funding mechanisms**: Different states balance revenue sources differently

### Data Suppression & Privacy
- The C2C dashboard suppresses data for groups with ≤10 students to protect privacy
- Trade-off: privacy protection vs. visibility for underrepresented communities
- Real-world implication: whose stories get told in data?

### From Data to Policy Questions
- Students learn to move from descriptive analysis ("what is the funding gap?") to evaluative questions ("is it equitable?") to prescriptive questions ("how should we fix it?")

## 🔗 External Resources

Students will use these tools during the lesson:

- **[edfinr R Package Documentation](https://urbaninstitute.github.io/edfinr/)**: Reference for data dictionary and function details
- **[C2C Student Pathways Dashboard](https://databydesign.caschooldashboard.org/)**: Interactive tool to explore California student outcomes by district
- **[C2C Data Portal](https://c2c.ca.gov/query-builder-student-pathways-dataset/)**: Download raw wage and outcome data

## 🤝 Contributing

This is my submission to the CA Cradle-2-Career Lesson Plan Challenge. Feedback and suggestions are welcome!

## 📄 License

This lesson plan and all associated materials are provided as an educational resource. The underlying data is from publicly available federal and California state sources.

---

**Questions or feedback?** Open an issue or reach out directly.

**Last updated**: March 2026
