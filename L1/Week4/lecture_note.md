# R Markdown

#### **Introduction to R Markdown**

*   **R Markdown**: A tool for creating reproducible documents combining text and code.
*   **Output Formats**: HTML, PDF, Word, and slides.
*   **Reproducibility**: Combines code, results, and explanations in one document, allowing others to replicate your analysis.

#### **Key Components of an R Markdown Document**

1.  **Header**:
    *   Defined by `---` at the top.
    *   Includes title, author, date, and output format (e.g., PDF).
2.  **Text Sections**:
    *   Uses Markdown syntax for formatting.
    *   **Bold**: `**text**`
    *   **Italics**: `*text*`
    *   **Headers**: `#` for H1, `##` for H2, etc.
3.  **Code Chunks**:
    *   Bounded by triple backticks ` ``` `
    *   Code is executed directly within the document.
    *   Output is included in the final document.
    *   **Shortcuts**:
        *   Insert code chunk: `Ctrl + Alt + I` (Windows) or `Cmd + Option + I` (Mac).
        *   Run a line of code: `Ctrl + Enter`.
        *   Run entire chunk: `Ctrl + Shift + Enter`.

#### **Formatting in R Markdown**

*   **Bold**: `**Bold**`
*   **Italicize**: `*Italic*`
*   **Headers**:
    *   `# H1 Header`
    *   `## H2 Header`
    *   `### H3 Header`
*   **Bulleted Lists**:
    *   Use `-` followed by a space.
    *   Ensure each line ends with two spaces to avoid spacing issues.

#### **Generating and Knitting**

*   **Knit Button**: Converts `.Rmd` file into the desired output format.
*   **File Save**: Save the document as an `.Rmd` file before knitting.
*   **PDF Rendering**: Outputs the final document with both text and executed code.

#### **Best Practices**

*   **Version Control**: Plain text format works well with Git, making it easy to track changes.
*   **Cheat Sheet**: Use the R Markdown cheat sheet provided by RStudio for advanced formatting and features.

#### **Example Workflow**

1.  Install the `rmarkdown` package: `install.packages("rmarkdown")`.
2.  Create a new R Markdown document: `File > New File > R Markdown`.
3.  Fill out the header, write text sections, and add code chunks.
4.  Knit the document to generate the final output (e.g., PDF).
5.  Use shortcuts and formatting tips to enhance document creation.

This summary covers the basics of creating, formatting, and rendering R Markdown documents, which will be useful for studying and preparing for your exam.

# Types of Data Science Questions

#### 1\. **Descriptive Analysis**

*   **Goal:** Describe or summarize a set of data.
*   **Key Concepts:**
    *   First step in data examination.
    *   Generates simple summaries about the samples and their measurements.
    *   **Examples:** Measures of central tendency (mean, median, mode), measures of variability (range, standard deviation).
    *   **Important Note:** This analysis is only for summarizing the data, not for making generalizations or interpretations.

#### 2\. **Exploratory Analysis**

*   **Goal:** Explore data to find relationships that weren't previously known.
*   **Key Concepts:**
    *   Identifies correlations but not causation.
    *   Useful for hypothesis generation and guiding future studies.
    *   **Example:** Analyzing the relationship between workforce participation of women in various sectors over time.
    *   **Important Note:** Exploratory analysis should not be used as the final say on data relationships.

#### 3\. **Inferential Analysis**

*   **Goal:** Use a sample of data to infer something about a larger population.
*   **Key Concepts:**
    *   Relies on statistical modeling.
    *   Involves estimating population values with a measure of uncertainty.
    *   **Examples:** Life expectancy studies related to air pollution.
    *   **Important Note:** Accurate inferences depend heavily on the representativeness of the sample.

#### 4\. **Predictive Analysis**

*   **Goal:** Use current data to make predictions about future data.
*   **Key Concepts:**
    *   Uses patterns in historical data to predict future outcomes.
    *   Requires measuring the right variables for accurate predictions.
    *   **Example:** Predicting election outcomes using polling data.
    *   **Important Note:** Prediction does not imply causation; accuracy is challenging to gauge before the event occurs.

#### 5\. **Causal Analysis**

*   **Goal:** Determine the cause-and-effect relationship between variables.
*   **Key Concepts:**
    *   Analyzes the impact of manipulating one variable on another.
    *   Common in randomized controlled trials (RCTs).
    *   **Example:** Studying the effect of a drug on infants with spinal muscular atrophy.
    *   **Important Note:** Causal analysis often involves aggregate data, and relationships may not apply to every individual.

#### 6\. **Mechanistic Analysis**

*   **Goal:** Understand the exact changes in variables leading to exact changes in other variables.
*   **Key Concepts:**
    *   Rarely used outside of physical and engineering sciences.
    *   Requires highly controlled variables and accurate measurements.
    *   **Example:** Studying how biocarbon particle size affects the mechanical properties of biodegradable plastics.
    *   **Important Note:** Best suited for deterministic equations; biological sciences are usually too noisy for mechanistic analysis.

# Experimental Design

#### **Introduction**
- **Experimental Design**: Organizing an experiment to collect correct and sufficient data for clear, effective answers to a data science question.
- **Importance**: Poor design can lead to incorrect conclusions, especially critical in fields like human health.

#### **Key Concepts**
- **Independent Variable (Factor)**: The variable manipulated by the experimenter. Displayed on the **x-axis**.
- **Dependent Variable**: The variable expected to change due to changes in the independent variable. Displayed on the **y-axis**.
- **Hypothesis**: An educated guess about the relationship between variables and the expected outcome of the experiment.

#### **Designing Experiments**
1. **Formulate the Question**: Clearly define what you want to answer before collecting data.
2. **Design Setup**: Plan how to gather data effectively and identify potential problems (e.g., sources of error).
3. **Confounders**: Extraneous variables that may affect the relationship between independent and dependent variables.
   - **Example**: Age as a confounder when studying the relationship between shoe size and literacy.
   - **Control for Confounders**: Measure and account for confounders, or fix them by controlling variables (e.g., fixing the age of participants).
4. **Sample Size**: Number of experimental subjects. Methods exist to determine the optimal sample size.

#### **Control Groups**
- **Purpose**: To compare the effects of a treatment with no treatment (control group).
- **Blinding**: Prevents subjects from knowing their group assignment to reduce bias (e.g., placebo effect).
- **Randomization**: Distributes confounders evenly across groups to minimize bias.

#### **Replication**
- **Definition**: Repeating an experiment with different subjects to confirm results.
- **Importance**: Strengthens the study's conclusions and allows for better assessment of data variability.

#### **Data Sharing**
- **GitHub**: A platform for sharing code and analysis. Important for transparency and reproducibility in science.

#### **P-Values and P-Hacking**
- **P-Value**: Probability that results occurred by chance.
  - **Significance Threshold**: Typically, a p-value < 0.05 is considered significant.
- **P-Hacking**: Exhaustively searching data to find statistically significant results by chance, leading to spurious correlations.
  - **Risk**: With big data, multiple tests increase the likelihood of finding misleading patterns.

#### **Final Notes**
- **Good Experimental Design**: Crucial to avoid erroneous conclusions.
- **P-Hacking**: Beware of manipulating data to achieve desired outcomes.


# Big Data

**Definition of Big Data:**
- **Big Data** refers to very large datasets characterized by three key qualities:
  - **Volume:** The sheer size of the data.
  - **Velocity:** The speed at which data is generated and processed.
  - **Variety:** The diversity of data types and sources.

**Evolution of Big Data:**
- **Data Storage Technology:** Advances in technology have allowed for the storage of increasingly larger datasets, expanding what is considered "big."
- **Data Collection Improvements:** The speed and methods for collecting data have improved, contributing to the rapid generation of large datasets.
- **Expansion of What Constitutes Data:** With the digital age, more types of interactions (e.g., social media, GPS, online behavior) are being recorded and considered as data.

**Structured vs. Unstructured Data:**
- **Structured Data:** Traditional data in organized formats like tables and databases (e.g., spreadsheets with rows and columns).
- **Unstructured Data:** Data not organized in a pre-defined manner (e.g., text, videos, social media interactions). This type of data is increasingly common and poses challenges in analysis.

**Challenges of Big Data:**
- **Size:** The enormous volume of data requires significant storage and processing capabilities.
- **Constant Change:** Data is continuously updating, making it difficult to have a static dataset for analysis.
- **Variety:** The numerous sources of data can make it difficult to determine the best data for analysis.
- **Messiness:** Unstructured data requires significant cleaning and structuring before analysis.

**Benefits of Big Data:**
- **Increased Accuracy:** Large datasets can help offset the effects of small errors or inaccuracies due to their volume.
- **Real-Time Analysis:** Constantly updating data allows for real-time analysis and decision-making.
- **New Insights:** Big Data can provide insights into previously unanswerable questions by leveraging new data sources.
- **Hidden Correlations:** Big Data can identify correlations that might not be obvious, aiding in predictive analysis.

**Limitations of Big Data:**
- **Not Always Useful:** Even with large datasets, they must be the right data to answer specific questions.
- **John Tukey’s Quote:** "The combination of some data and an aching desire for an answer does not ensure that a reasonable answer can be extracted from a given body of data." This emphasizes the importance of having relevant data for your specific question.

**Key Takeaways:**
- **Big Data’s Characteristics:** Volume, velocity, and variety.
- **Importance of Data Relevance:** The size of the dataset does not guarantee that it is appropriate for answering your specific question.
- **Structured vs. Unstructured Data:** Understanding the difference and challenges of unstructured data.
- **Challenges and Benefits:** Recognize the potential difficulties and advantages in working with Big Data.
- **Real-Time Analysis & Hidden Correlations:** Big Data can provide real-time insights and uncover hidden relationships.
