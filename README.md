# Data Science and AI-Assisted Programming

A hands-on tutorial designed for social science researchers, aimed at bridging the gap between traditional theoretical analysis and modern data science. Using CGSS 2023 micro-survey data as a practical carrier, it systematically explains how to use programming tools and AI-assisted technologies to achieve a fully reproducible research workflow—from data cleaning to machine learning modeling—helping researchers conduct quantitative analysis efficiently and rigorously.

## 📚 Table of Contents

### 1. Introduction to Data Science and AI-Assisted Programming

This chapter redefines the role of data science in social science: it is not just a collection of sophisticated algorithms, but a way of thinking to extract patterns from massive, messy data.

**Key Concepts:**
- **Data Science in Social Science**: Moving beyond traditional text analysis to pattern extraction from large-scale data
- **Core Components**: Four essential stages of data science workflow
  - Data acquisition and reading
  - Data cleaning (the most time-consuming step)
  - Exploratory analysis
  - Statistical modeling
- **AI-Assisted Programming**: Revolutionizing traditional research paradigm
  - Eliminates the need to memorize code syntax
  - Allows researchers to focus on research question definition
  - Enables logical construction without technical barriers

**Benefits:**
- Lower barrier to entry for social science researchers
- Shift from "memorizing code" to "defining research problems"
- Improved reproducibility and documentation

---

### 2. Setting up Environment: Installing VSCode and Plugins (or Trae)

Two battle-tested environment configuration options are provided to suit different preferences:

#### Option A: VS Code + Plugin Ecosystem

The global standard for data scientists, offering unparalleled extensibility.

**Setup Steps:**
1. **Python Installation**
   - Download from official Python website
   - Ensure "Add Python to PATH" is checked during installation
   
2. **VS Code Installation**
   - Download from VS Code official website
   - Configure Chinese language pack if needed
   
3. **Core Plugin Installation**
   - **Python**: Enables VS Code to recognize Python language
   - **Jupyter**: Allows running code in segments with immediate visualization
   - Search and install from VS Code Extension Marketplace
   
4. **AI Programming Assistant**
   - Activate Copilot for Gemini, Claude, and GPT-4o support
   - This is the key difference from traditional programming
   
5. **Domestic Mirror Configuration**
   - Configure Alibaba/Tsinghua mirror for faster package downloads
   - Ensure stable and efficient environment

**Advantages:**
- Maximum extensibility and customization
- Large community support
- Rich plugin ecosystem

#### Option B: TraeCN (AI-Native Editor)

A minimalist tool optimized for data science with built-in AI capabilities.

**Setup Steps:**
1. **Python Installation**
   - Same requirements as Option A
   - Critical: Must check "Add Python to PATH"
   
2. **TraeCN Installation**
   - Download from Trae official website
   - Default installation process
   - Automatic language detection (Chinese/English)
   
3. **Intelligent Configuration**
   - Automatic plugin installation
   - One-click Python and Jupyter setup
   - No manual plugin searching required
   
4. **Built-in AI Assistant**
   - Located in sidebar (chat bubble icon)
   - No additional setup needed
   - Two modes:
     - **Chat Mode**: Like a teacher answering questions
     - **Builder Mode**: Like a worker creating files and code (frequently used)

**Advantages:**
- Minimal setup time
- Built-in AI integration
- Optimized for data science workflows
- Lower learning curve

---

### 3. Data Input and Cleaning

Using CGSS 2023 data as an example, this is the most time-consuming but critical step.

**Learning Objectives:**

#### 3.1 Data Reading
- **Efficient Format Handling**
  - Read professional formats like `.dta` (Stata format)
  - Preserve complete metadata (e.g., variable labels)
  - Handle large datasets efficiently
  
- **Tools and Methods**
  - Using pandas for data import
  - Understanding data structure and variable types

#### 3.2 Missing Value Identification
- **CGSS-Specific Codes**
  - Recognize special missing value codes:
    - `98`: "Don't know"
    - `99`: "Refuse to answer"
    - `-8`: "Not applicable"
  - Prevent distortion of statistical results
  
- **Handling Strategies**
  - Convert special codes to proper missing values
  - Apply logical rules for data cleaning
  - Document all transformations

#### 3.3 Reproducible Scripts
- **Best Practices**
  - Write clear, documented cleaning scripts
  - Maintain research workflow documentation
  - Enable peer review and self-review
  - Ensure full reproducibility

**Key Takeaways:**
- Data cleaning is foundational to research quality
- Proper missing value handling prevents biased results
- Documented scripts enable transparency

---

### 4. Descriptive Statistics and Visualization

"Seeing" the story in data through systematic exploration.

**Core Components:**

#### 4.1 Basic Descriptive Statistics
- **Measures of Central Tendency**
  - Mean, median, mode
  - Understanding data distribution
  
- **Measures of Dispersion**
  - Standard deviation
  - Variance
  - Range and interquartile range
  
- **Frequency Analysis**
  - Count and percentage distributions
  - Cross-tabulations

#### 4.2 Data Visualization
- **Distribution Plots**
  - Histograms: Show frequency distribution
  - Density plots: Smooth distribution curves
  - Boxplots: Identify outliers and quartiles
  
- **Comparative Visualizations**
  - Bar charts: Compare categories
  - Grouped plots: Show relationships
  
- **Benefits**
  - Intuitively present variable distributions
  - Quickly identify outliers
  - Understand data characteristics

**Applications:**
- Initial data exploration
- Quality assessment
- Pattern identification
- Communication of findings

---

### 5. Bivariate and Multivariate Analysis, Table Output and Visualization

Exploring relationships between variables systematically.

#### 5.1 Bivariate Analysis
- **Statistical Tests**
  - **Chi-square tests**: Test independence between categorical variables
  - **Pearson correlation**: Linear relationship between continuous variables
  - **Spearman correlation**: Monotonic relationship between ordinal variables
  
- **Cross-tabulations**
  - Frequency tables for categorical relationships
  - Conditional distributions

#### 5.2 Multivariate Relationship Visualization
- **Advanced Plotting Techniques**
  - **Scatter plots**: Show relationship between two continuous variables
  - **Heatmaps**: Visualize correlation matrices
  - **Grouped bar charts**: Compare across multiple categories
  - Faceted plots: Show patterns across subgroups

#### 5.3 Academic Standard Tables
- **Professional Formatting**
  - APA style tables
  - Coefficient tables with standard errors
  - Significance indicators (*, **, ***)
  
- **Direct Usage**
  - Ready for research papers
  - Meets journal requirements
  - Consistent with academic standards

**Research Applications:**
- Hypothesis testing
- Relationship exploration
- Pattern discovery
- Result communication

---

### 6. Linear Regression Model Analysis, Multivariate Analysis, Tables and Visualization

In-depth application of classical linear regression (OLS).

#### 6.1 Model Specification and Estimation
- **Model Building**
  - Define dependent and independent variables
  - Choose appropriate functional form
  - Specify control variables
  
- **Estimation Methods**
  - Ordinary Least Squares (OLS)
  - Understanding regression coefficients
  - Interpreting statistical significance

#### 6.2 Model Diagnostics
- **Assumption Checking**
  - **Multicollinearity**: Check VIF (Variance Inflation Factor)
  - **Heteroskedasticity**: Test for constant variance
  - Normality of residuals: Assess error distribution
  
- **Remedial Actions**
  - Variable transformation
  - Robust standard errors
  - Model specification adjustments

#### 6.3 Advanced Features
- **Dummy Variables**
  - Handling categorical predictors
  - Reference category selection
  - Interpretation of categorical coefficients
  
- **Interaction Terms**
  - Modeling conditional relationships
  - Testing moderation effects
  - Interpreting interaction coefficients

#### 6.4 Professional Results Presentation
- **Visualization Techniques**
  - **Coefficient plots**: Show effect sizes with confidence intervals
  - **Marginal effect plots**: Display predicted values
  - Forest plots: Compare multiple models
  
- **Benefits**
  - Make regression results more persuasive
  - Enhance interpretability
  - Facilitate peer understanding

**Research Impact:**
- Rigorous causal inference
- Transparent methodology
- Clear communication of findings

---

### 7. Generalized Regression Model Analysis

When the dependent variable is no longer continuous.

#### 7.1 Binary Dependent Variables
- **Logit/Probit Regression**
  - Analyzing dichotomous outcomes
  - Example: "participation vs. non-participation"
  - Understanding odds ratios and marginal effects
  
- **Applications**
  - Binary choice models
  - Probability estimation
  - Policy evaluation

#### 7.2 Ordinal Dependent Variables
- **Ordered Logit/Probit Regression**
  - Handling ordered categorical outcomes
  - Example: "satisfaction ratings" (1-5 scale)
  - Respecting ordinal nature of data
  
- **Interpretation**
  - Threshold parameters
  - Cumulative probabilities
  - Latent variable framework

#### 7.3 Model Assessment
- **Goodness-of-Fit Measures**
  - Pseudo R-squared
  - Likelihood ratio tests
  - Information criteria (AIC, BIC)
  
- **Model Comparison**
  - Nested model tests
  - Predictive accuracy
  - Model selection criteria

**Research Applications:**
- Survey data analysis
- Choice modeling
- Satisfaction studies
- Policy impact assessment

---

### 8. Decision Trees and Machine Learning

Stepping into the world of machine learning.

#### 8.1 Tree-Based Methods
- **Decision Trees**
  - Working principles: Recursive partitioning
  - Advantages: Interpretability, non-linearity
  - Visualization of decision rules
  
- **Random Forests**
  - Ensemble learning approach
  - Improved prediction accuracy
  - Feature importance assessment

#### 8.2 Model Training and Evaluation
- **Training Process**
  - Train-test split
  - Cross-validation
  - Hyperparameter tuning
  
- **Performance Metrics**
  - **Accuracy**: Overall correct classification rate
  - **Confusion matrices**: True/false positives/negatives
  - Precision, recall, F1-score
  - ROC curves and AUC

#### 8.3 Model Interpretability
- **Feature Importance**
  - Ranking variable contributions
  - Understanding predictive drivers
  - Enhancing research conclusions
  
- **Explainability**
  - SHAP values
  - Partial dependence plots
  - Individual prediction explanations

**Research Benefits:**
- Capture complex, non-linear relationships
- Improve predictive performance
- Identify key predictors
- Ensure reliability of conclusions

---

## 📊 Core Data and Case Studies

### Primary Dataset
- **File**: `cgss2023.dta`
- **Description**: The 2023 microdata from Chinese General Social Survey
- **Coverage**: Multiple dimensions including:
  - Demographics (age, gender, education)
  - Economics (income, employment)
  - Social attitudes and values
- **Role**: Practical carrier throughout the entire tutorial

### Complete Analysis Notebook
- **File**: `ChineseVersion中文完整版分析.ipynb`
- **Contents**: 
  - Complete Chinese Jupyter Notebook
  - All code from data reading to modeling
  - Detailed comments and explanations
  - Result interpretations
- **Purpose**: Best practice for quick start and reference

---

## 🎯 Target Audience

### Primary Users
- **Graduate Students**: In social science disciplines
  - Sociology
  - Public Administration
  - Political Science
  - Economics
  
- **Young Scholars**: Researchers seeking to modernize methods
  - Improve research efficiency
  - Enhance analytical rigor
  - Adopt reproducible workflows

### Secondary Users
- **Researchers**: Using modern data science methods
  - Quantitative analysis enhancement
  - Advanced statistical techniques
  - Machine learning applications

- **Beginners**: Interested in AI-assisted programming
  - Lower barrier to entry
  - Focus on research itself
  - Learn practical skills

---

## 📄 License

This project is licensed under **MIT License**.

**Permissions:**
- ✅ Learn: Use for educational purposes
- ✅ Use: Apply in research and projects
- ✅ Share: Distribute to others
- ✅ Build upon: Modify and extend for innovation

**Encouragement:**
Everyone is welcome to learn, use, share, and build upon this project for further development and innovation in social science research.

---

## 🚀 Getting Started

### Quick Start Guide
1. **Choose Your Environment**: Select VS Code or Trae based on your preference
2. **Install Dependencies**: Follow the setup instructions for your chosen environment
3. **Download Data**: Obtain CGSS 2023 dataset
4. **Open the Notebook**: Start with the complete Chinese version
5. **Follow the Tutorial**: Work through each chapter sequentially
6. **Experiment**: Modify code and explore different analyses

### Support and Resources
- **Documentation**: Detailed explanations in each notebook
- **Code Comments**: Comprehensive inline documentation
- **Examples**: Real-world applications throughout
- **Community**: Join discussions and share insights

---

## 📝 Contributing

We welcome contributions from the community!

**Ways to Contribute:**
- Report bugs and issues
- Suggest new features
- Improve documentation
- Share examples and case studies
- Submit pull requests

**Guidelines:**
- Follow the existing code style
- Add clear documentation
- Test your changes thoroughly
- Respect the project's educational mission

---

## 📞 Contact

For questions, suggestions, or collaboration opportunities, please reach out through the project repository.

---

*Happy analyzing! May your research be rigorous, reproducible, and impactful.* 🎓📊
