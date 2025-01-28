# Amazon Review Analysis

This project analyzes Amazon product reviews to validate various hypotheses related to review scores, helpfulness ratios, and user behavior. The dataset used contains **568,454 reviews**, and the analysis was performed using **Python** with libraries such as `pandas`, `numpy`, `matplotlib`, and `seaborn`.

## Project Structure

### 1. Data Loading and Cleaning
- Loaded the dataset from `Reviews.csv`.
- Cleaned the dataset by handling missing values and converting the `Time` column to a datetime format.
- Removed duplicate entries to ensure data quality.

### 2. Hypothesis Analysis
The following hypotheses were tested:

1. **Review scores are generally positive**  
   - Analyzed the distribution of review scores.
   - Majority of reviews have a score of `5`, contributing to 63.87% of all reviews.  
   **Conclusion:** Hypothesis is **true**.

2. **Helpful reviews are often marked as such by many users**  
   - Investigated the correlation between `HelpfulnessNumerator` and `HelpfulnessDenominator`.
   - Found a strong positive correlation (r ≈ 0.97).  
   **Conclusion:** Hypothesis is **true**.

3. **There are differences in review scores among different products**  
   - Grouped reviews by `ProductId` to calculate average scores.
   - Found varying scores across products.  
   **Conclusion:** Hypothesis is **true**.

4. **Length of the review text correlates with the review score**  
   - Performed correlation analysis between review length and scores.
   - Found a weak negative correlation (r ≈ -0.077).  
   **Conclusion:** Hypothesis is **false**.

5. **Certain users are more active in leaving reviews**  
   - Identified top reviewers and their contribution.
   - Observed significant differences in review counts among users.  
   **Conclusion:** Hypothesis is **true**.

6. **Reviews have become more detailed over time**  
   - Analyzed the average text length of reviews by year.
   - Found no consistent upward trend.  
   **Conclusion:** Hypothesis is **false**.

7. **High-rated reviews receive more helpfulness votes**  
   - Grouped reviews by `Score` to compare helpfulness votes.
   - Found that reviews with higher scores have more helpfulness votes.  
   **Conclusion:** Hypothesis is **true**.

8. **Products with more reviews tend to have higher average scores**  
   - Analyzed the relationship between review count and average scores.
   - Found a negative correlation.  
   **Conclusion:** Hypothesis is **false**.

9. **Negative reviews are often shorter than positive reviews**  
   - Compared the average text length of negative and positive reviews.
   - Found negative reviews to be longer on average.  
   **Conclusion:** Hypothesis is **false**.

10. **Review scores and helpfulness ratios differ across products**  
    - Analyzed top 10 products based on helpfulness ratios and average scores.
    - Found significant differences.  
    **Conclusion:** Hypothesis is **true**.

### 3. Visualization
- Plots such as histograms, scatter plots, line charts, and bar charts were created to support the analysis.
- Example visualizations:
  - Distribution of review scores
  - Helpfulness ratios across reviews
  - Average text length over time
  - Comparison of helpfulness votes for different scores

### 4. Tools and Libraries
- **Python**: Core programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Statistical analysis
- **Matplotlib** and **Seaborn**: Data visualization
- **VADER Sentiment Analysis**: Sentiment classification of reviews

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/Arjun-Menon2110/Amazon-Review-Analysis.git
