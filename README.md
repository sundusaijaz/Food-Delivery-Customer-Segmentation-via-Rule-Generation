### Food Delivery Rules Generation Summary

This project utilized unsupervised learning techniques, particularly the Apriori algorithm, to generate rules for potential customers of food delivery services. The rules were based on a variety of customer metadata, including income, travel habits, outgoing behaviors, tipping practices, delivery costs, distances between homes and restaurants, marital status, and occupational status.

#### Project Insights

- **Dataset Summary:**
  - Total dataset size: 1571 rows and 46 columns.
  - After filtering out the last three columns, the dataset remained with columns from ID to 'Why do you not use delivery applications?' (332 rows and 46 columns).

- **Data Processing:**
  - The dataset underwent Association Rule mining by converting it into Transactional Data through a form of One-Hot Encoding.
  - The resulting dataset consisted of 332 rows and 1058 columns.
  - A total of 8,461,441 rules were produced through Association Rules mining.

- **Rule Criteria:**
  - The rules were further refined based on specific criteria:
    - Support > 0.2
    - Confidence >= 0.7
    - Lift > 1.0

- **Rule Categorization:**
  - Rules were categorized for females and males based on lift, support, and confidence.

#### Findings:

**For Females:**
1. Females valuing customer service highly tend to prioritize timing accuracy, driving, working spouses, having a maid at home, using delivery applications, Saudi nationality, and emphasizing delivery cost.
2. Those valuing discount offers highly display similar behavioral patterns to the first group.
3. Females prioritizing delivery speed exhibit similar tendencies as the other groups.

**For Males:**
1. Single male students with Saudi nationality and lower income levels tend to drive, have a working spouse, employ a maid at home, and use delivery applications.
2. Single males with lower income levels demonstrate similar tendencies as the first group.
3. Male respondents valuing timing accuracy and delivery cost also show preferences for discount offers, delivery speed, driving, having a working spouse, employing a maid at home, and using delivery applications.

#### GitHub Repository Abstract

The repository contains Python code implementing unsupervised learning, specifically the Apriori algorithm, applied to a dataset containing customer metadata for food delivery. It showcases the dataset details, data processing methods, Association Rule generation, and the interpretation of the significant rules extracted for both female and male customers.

The repository demonstrates an in-depth analysis of customer behaviors and preferences, essential for targeted food delivery services and customer segmentation. The findings provide valuable insights for businesses seeking to optimize their service offerings based on distinct customer preferences and characteristics.

### Tools and Algorithms Utilized:
- **Tools:** Python, Pandas, NumPy
- **Algorithm:** Apriori algorithm for Association Rule mining

This abstract serves as a quick reference to the repository's content, methods used, and the insights derived from the analysis of customer metadata in the context of food delivery services. The detailed results, interpretations, and implications for food delivery businesses are available within the repository.
