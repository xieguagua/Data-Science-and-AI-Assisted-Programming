# Part One: What is Data Science?

In the traditional humanities context, we emphasize close reading or theoretical speculation. In the data science context, we emphasize extracting patterns from massive, messy data.

Data science is not just about sophisticated algorithms. It mainly consists of four core components:

---

## 1. Data Acquisition and Loading

**Traditional pain point:** CGSS data is usually in Stata (.dta) format, which cannot be opened in Excel and loads very slowly in SPSS.

**Solution through programming:** We can instantly read data files with tens of thousands of rows and hundreds of columns, while preserving all metadata (e.g., the variable label "A36" stands for "happiness").

---

## 2. Data Cleaning — the most time-consuming step

**Scenario (specific to CGSS):**
- In CGSS,
  - "Don't know" is coded as 98,
  - "Refuse to answer" is coded as 99,
  - "Not applicable" is coded as -8.

**Issue:** If you calculate the mean directly without handling these values, a score of 99 will severely distort your results.

**Data science perspective:**
We write logic to instruct the computer: "If the value of variable A is in the list [98, 99, -8], treat it as a missing value and exclude it from calculations."

**Advantage:**
This ensures reproducibility and preserves the workflow of your research.

---

## 3. Exploratory Data Analysis

**Scenario:** You want to know whether there is a relationship between income and happiness.

**Data science perspective:**
Instead of running regressions directly, we first conduct basic descriptive analysis, then create visualizations (scatter plots, heatmaps). Through visualization, we intuitively observe data distributions and identify outliers.

---

## 4. Statistical Modeling

**Scenario:** Testing hypotheses.

**Data science perspective:**
From simple OLS regression to complex machine learning models.

---

# Part Two: What is AI-assisted Programming?

The emergence of AI-assisted programming (LLM-based code generation) is not simply "automatic code writing". It enables a new paradigm of human–computer collaborative research.

---

## 1. Core principle: Semantic-based logical mapping

**Traditional programming:** Requires researchers to master computer syntax to communicate with machines.

**AI-assisted programming:** Allows researchers to describe research goals in natural language, and the large language model maps "research intent" to "executable code" behind the scenes.

**Traditional mode:**
- Researcher thinking: "I need to clean the data."
- Cognitive barrier: Must memorize code such as `df.loc[df['income'] < 0, 'income'] = np.nan`

**AI-assisted mode:**
- Researcher thinking: "Code negative values in the income variable as missing values."

**Abstraction upgrade:**
You only define logical rules; AI handles implementation details.

**Academic implication:**
The threshold for programming has shifted from memorizing code to clearly defining research questions.

---

## 2. Three functional dimensions of AI in quantitative research

When analyzing complex micro-survey data such as CGSS 2023, AI plugins serve three academic roles:

### Role A: Operationalization executor
The core of sociological research is translating abstract concepts into measurable indicators. AI quickly converts your operational definitions into code.

### Role B: Interactive error diagnostics
Program errors often reflect logical inconsistencies or environment mismatches. AI acts as a technical reviewer.

### Role C: Methodological best-practice consultant
This is AI's most promising high-level function. Drawing on massive code repositories and statistical documentation, it provides recommendations aligned with mainstream academic standards.