<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Going Beyond Correlation to Causation</title>
</head>
<body>
    <h1>Project Overview</h1>
    <h2>Going Beyond Correlation: Finding Patterns to Causation</h2>
    <p><strong>Objective:</strong> Explore how to identify causal relationships in data, moving beyond simple correlations to uncover true causal effects.</p>
    <p><strong>Goal:</strong> Use causal inference techniques to determine if changes in <em>X</em> lead to changes in <em>Y</em>.</p>
    <p><strong>Why this matters:</strong> Causal inference helps establish true cause-and-effect relationships, which are essential for making informed decisions in fields like healthcare, economics, and social sciences.</p>

    <h2>Research Question(s)</h2>
    <ul>
        <li><strong>What is the causal relationship between <em>X</em> and <em>Y</em>?</strong><br>
            - Are there any direct or indirect causal paths from <em>X</em> to <em>Y</em>?</li>
        <li><strong>How can observational data help identify causality?</strong><br>
            - How can we overcome the limitations of non-experimental data to estimate causal effects?</li>
        <li><strong>What confounding factors influence the relationship between <em>X</em> and <em>Y</em>?</strong><br>
            - Are there other variables that affect both <em>X</em> and <em>Y</em>, potentially distorting the causal inference?</li>
    </ul>

    <h2>Hypothesis</h2>
    <ul>
        <li><strong>Hypothesis 1:</strong><br>
            - <em>X</em> directly influences <em>Y</em>. If we manipulate <em>X</em>, we expect <em>Y</em> to change in a measurable way.</li>
        <li><strong>Hypothesis 2:</strong><br>
            - There are confounders (variables <em>Z</em>) that may affect both <em>X</em> and <em>Y</em>, and we need to control for these to get an accurate estimate of the causal effect.</li>
        <li><strong>Hypothesis 3:</strong><br>
            - Quasiexperimental techniques (e.g., propensity score matching) will help mitigate confounding biases and provide a more reliable estimate of the causal effect of <em>X</em> on <em>Y</em>.</li>
    </ul>

    <h2>Causal Diagram</h2>
    <p><em>X</em>: Independent variable (e.g., intervention or treatment)<br>
       <em>Y</em>: Dependent variable (e.g., outcome or result)<br>
       <em>Z</em>: Confounding variables (e.g., third variables affecting both <em>X</em> and <em>Y</em>)</p>
    <pre>
      Z   ----->  X  -----> Y
      |               ^
      |_______________|
    </pre>

    <h2>Quasiexperimental Techniques</h2>
    <h3>1. Propensity Score Matching (PSM)</h3>
    <p><strong>Objective:</strong> Estimate causal effects by matching treated units with non-treated units based on similar characteristics.</p>
    <p><strong>Plan:</strong> Step-by-step implementation to compare treatment and control groups in terms of propensity scores.</p>

    <h3>2. Inverse Propensity Score Weighting (IPSW)</h3>
    <p><strong>Objective:</strong> Address selection bias by giving more weight to underrepresented units based on the inverse of their propensity scores.</p>
    <p><strong>Plan:</strong> Use weighting to adjust for treatment assignment and estimate causal effects.</p>

    <h2>Data Collection</h2>
    <h3>Data Sources:</h3>
    <ul>
        <li>Where is the data coming from? (e.g., public datasets, company data, surveys, etc.)</li>
        <li><strong>Key Variables:</strong> Describe the key variables (e.g., <em>X</em>, <em>Y</em>, <em>Z</em>), and their operational definitions.</li>
    </ul>

    <h3>Data Cleaning & Preparation:</h3>
    <ul>
        <li>List steps for cleaning data, handling missing values, outliers, and preparing it for analysis.</li>
    </ul>

    <h2>Analytical Plan</h2>
    <h3>Step 1: Exploratory Data Analysis (EDA)</h3>
    <ul>
        <li>Inspect the data for any patterns, correlations, or anomalies.</li>
        <li>Visualize distributions and relationships between key variables.</li>
    </ul>

    <h3>Step 2: Estimate Propensity Scores</h3>
    <ul>
        <li>Use logistic regression (or other techniques) to estimate the probability of treatment for each observation based on observed covariates.</li>
    </ul>

    <h3>Step 3: Implement Propensity Score Matching</h3>
    <ul>
        <li>Match treated units with control units based on the estimated propensity scores.</li>
    </ul>

    <h3>Step 4: Apply Inverse Propensity Score Weighting (if needed)</h3>
    <ul>
        <li>Calculate weights for each unit and adjust the analysis to account for the selection bias.</li>
    </ul>

    <h3>Step 5: Estimate Causal Effects</h3>
    <ul>
        <li>Compare outcomes between treatment and control groups (with appropriate adjustments) to estimate the causal effect of <em>X</em> on <em>Y</em>.</li>
    </ul>

    <h2>Results (to be filled in as you conduct the study)</h2>
    <h3>Descriptive Statistics:</h3>
    <ul>
        <li>Overview of key statistics from the data (mean, median, variance, etc.).</li>
    </ul>

    <h3>Results of Propensity Score Matching:</h3>
    <ul>
        <li>Describe the matching process and any results from comparing treated and untreated units.</li>
    </ul>

    <h3>Causal Estimation:</h3>
    <ul>
        <li>Estimate and interpret the causal effect of <em>X</em> on <em>Y</em>. Consider the significance and magnitude of the effect.</li>
    </ul>

    <h2>Discussion</h2>
    <h3>Interpretation of Results:</h3>
    <ul>
        <li>What do the findings suggest about the causal relationship between <em>X</em> and <em>Y</em>?</li>
    </ul>

    <h3>Limitations:</h3>
    <ul>
        <li>Discuss potential limitations of the study, such as unobserved confounders or limitations in the data.</li>
    </ul>

    <h3>Implications:</h3>
    <ul>
        <li>What do the findings mean for theory, practice, or policy?</li>
    </ul>

    <h2>Conclusion (to be written at the end of the study)</h2>
    <h3>Summary of Findings:</h3>
    <ul>
        <li>Recap the main findings regarding the causal relationship between <em>X</em> and <em>Y</em>.</li>
    </ul>

    <h3>Future Research:</h3>
    <ul>
        <li>What additional questions remain? What improvements or future studies could be conducted to build upon this work?</li>
    </ul>
</body>
</html>
