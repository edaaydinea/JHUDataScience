# What is Data Science?

1. **Definition of Data Science:**
    - **Core Concept:** Using data to answer questions.
    - **Scope:** Includes statistics, computer science, mathematics, data cleaning, formatting, and visualization.
2. **Skills of a Data Scientist:**
    - **Venn Diagram Intersection:**
        - **Substantive Expertise:** Knowledge in the area of interest.
        - **Hacking Skills:** Programming and data manipulation.
        - **Math and Statistics:** Analytical and statistical skills.
3. **Importance of Data Science:**
    - **Rise in Data:** Increased data availability and inexpensive computing.
    - **Historical Context:** From the Library of Alexandria to modern data volume.
    - **Big Data Characteristics:**
        - **Volume:** Large datasets (e.g., YouTube uploads).
        - **Velocity:** Rapid data generation and collection.
        - **Variety:** Different types of data (e.g., structured vs. unstructured).
4. **Role of a Data Scientist:**
    - **Basic Definition:** Uses data to answer questions.
    - **Skills Focus:**
        - **Programming:** Using R for data access, analysis, and visualization.
        - **Problem Solving:** Finding answers to novel problems.
5. **Demand for Data Scientists:**
    - **Growing Roles:** Increased demand in machine learning, data science, and big data.
    - **Supply and Demand:** Demand exceeds supply (650% growth since 2012).
    - **Top Job:** Data scientist ranked as the top job in the US in 2017 by Glassdoor.
6. **Examples of Data Scientists:**
    - **Daryl Morey:** GM of Houston Rockets, leveraging data for hiring decisions.
    - **Hilary Mason:** Co-founder of FastForward Labs, focusing on web data and social media.
    - **Nate Silver:** Founder of FiveThirtyEight, known for using data to predict elections and other topics.
7. **Case Study:**
    - **Google Flu Trends (2009):** Analyzed search terms to predict flu outbreaks, identifying 45 correlated words with CDC data.
8. **Course Overview:**
    - **R Programming:** Basics and installation.
    - **RStudio:** Graphical interface to R.
    - **Version Control:** Importance and integration.
    - **Application:** Using tools to answer data science questions.

# What is data?

1. **Definition by Cambridge English Dictionary:**
    - Data is information, especially facts or numbers.
    - Collected to be examined, considered, and used for decision-making.
2. **Definition by Wikipedia:**
    - A set of values of qualitative or quantitative variables.
    - Data comprises values, numbers, or facts.
    - Collected, examined, and used to inform decisions.
3. **Components of Data:**
    - A set of items to measure from (often called population in statistics).
    - Variables are measurements or characteristics of an item.
    - Qualitative variables: Information about qualities (e.g., country of origin, sex).
    - Quantitative variables: Information about quantities (e.g., height, weight).
4. **Data Examples:**
    - Basic examples: Country of origin, sex, height, weight.
    - Often presented in a tidy spreadsheet format with rows and columns.
5. **Messiness of Data:**
    - Data sets are usually not tidy.
    - Tasks include extracting information, organizing it into a tidy format, analyzing it, and visualizing results.
6. **Types of Data:**
    - Sequencing Data:
        - Encountered in fast queue format.
        - Hundreds of millions of lines long.
        - Parsed into an understandable format to infer genomic information.
        - Example: Expression data producing a Volcano Plot.
    - Census Data:
        - Standardized questions answered by almost all members of a country.
        - Large and messy but valuable once queried.
        - Example: US Census results plotted in a population pyramid plot.
    - Electronic Medical Records:
        - Popular way to store health information.
        - Used in population-based studies to answer questions and improve medical care.
        - Example: Extracting allergy information into a table format for analysis.
    - Image/Video Data:
        - Rich information coded in images/videos waiting to be extracted.
        - Example: Facebook’s face recognition and Google’s Deep Dream software.
7. **Question-First Approach:**
    - Data is important but secondary to the question.
    - A good data scientist asks questions first and seeks relevant data second.
    - Available data may limit or enable certain questions.
    - The data itself does not drive the question asking.
8. **Summary:**
    - Definitions of data focus on actions surrounding data and what comprises data.
    - Concepts of populations and variables with qualitative and quantitative data differences.
    - Different data sources emphasize the lack of tidy data sets.
    - Importance of question-first strategies in data science.

# Getting Help

1. **Importance of Problem-Solving**:
    - Problem-solving is a fundamental skill in data science.
    - This course involves thousands of students, making immediate help from instructors impractical.
    - Solving problems independently is crucial for a data scientist.
2. **Transferable Skill**:
    - Troubleshooting and finding solutions is valuable in any career.
3. **Initial Steps for Solving Problems**:
    - **Read Manuals/Help Files**: Use the help command (e.g., question mark command) to find answers.
    - **Search Online**: Use Google and relevant forums like Stack Overflow and Cross Validated.
    - **Course Forum**: Utilize the course forum for class-specific questions.
4. **Dealing with Coding Problems**:
    - **Error Messages**:
        - Check for typos.
        - Read error messages carefully.
    - **Unexpected Output**:
        - Analyze how the output differs from expectations.
        - Understand what the command actually did.
5. **Getting Help from Others**:
    - **Ask Peers**: Engage with classmates or experienced peers.
    - **Rubber Duck Debugging**: Explain the problem to an inanimate object or a non-expert to find a solution.
6. **Posting Questions on Forums**:
    - **Details to Include**:
        - Specific question and troubleshooting steps taken.
        - How to reproduce the problem and sample data.
        - Expected vs. actual output.
        - Relevant system/product details.
    - **Title**: Make it specific to attract relevant help.
7. **Forum Etiquette**:
    - **Dos**:
        - Ask in the appropriate forum.
        - Be explicit and detailed.
        - Provide necessary information.
        - Be courteous.
        - Follow up with the solution.
    - **Don'ts**:
        - Avoid assuming program faults.
        - Don't expect others to do your homework.
        - Avoid cross-posting the same question on multiple forums.
8. **Conclusion**:
    - Effective problem-solving and help-seeking are crucial in data science.
    - Practice solving problems to improve these skills.

# Data Science Process

1. **Introduction to Data Science Projects**
    - Discussion on what data and data science are.
    - Importance of knowing the steps in a data science project.
2. **Steps in a Data Science Project**
    - **Formulating the Question**
        - The question guides the data collection and analysis.
        - Example: Hilary Parker's question about the name "Hilary".
    - **Collecting Data**
        - Data is needed to answer the question.
        - Example: Data from the Social Security website on baby names from 1880 to 2011.
    - **Analyzing the Data**
        - Explore and model the data to draw conclusions.
        - Example: Calculating relative risk for baby names year by year.
    - **Communicating Results**
        - Share findings through reports, blog posts, or presentations.
        - Example: Hilary Parker’s blog post detailing her findings.
3. **Example Project: Hilary Parker's Analysis**
    - **Question:** Is "Hilary" the most rapidly poisoned name in recorded American history?
    - **Data Collection:** 1,000 most popular baby names from 1880-2011 from the Social Security website.
    - **Data Analysis:**
        - Calculation of relative risk for each name.
        - Identification of names with the biggest drop in popularity.
    - **Findings:** "Hilary" had the quickest fall in popularity among names that were popular for more than 20 years.
    - **Communication:** Blog post detailing the analysis and results.
4. **Coding and Analysis Process**
    - Writing code to gather and format data.
    - Generating figures and running analyses.
    - Code available on GitHub for reproducibility.
5. **Communicating Results Effectively**
    - Writing detailed blog posts or reports.
    - Providing credit to sources and previous work.
    - Example: Hilary Parker linked to sources and explained her methods.
6. **Additional Data Science Projects Examples**
    - **Opioid Overdose Risk Prediction:** Project by University of Pennsylvania students using R.
    - **Living Preferences by Weather:** Analysis by Maelle Samuel.
    - **Trump’s Tweets Analysis:** Work by David Robinson.
    - **Toronto Sexual Health Clinics Map:** Project by Charlotte Galvin.
