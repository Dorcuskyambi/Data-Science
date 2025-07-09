IBM Applied Data Science Capstone Project
Presentation Slides: Available in Capstone_Presentation.pdf

Executive Summary
This capstone project focuses on predicting whether the SpaceX Falcon 9 first stage will land successfully using various machine learning classification models. The key steps include:

Data collection, cleaning, and formatting

Exploratory data analysis (EDA)

Interactive visualizations

Machine learning predictions

Our analysis reveals correlations between certain launch features (e.g., payload mass, orbit type) and mission success. Among the tested algorithms, the decision tree model performed best in predicting landing outcomes.

Introduction
SpaceX offers Falcon 9 launches at $62 million, significantly lower than competitors (over $165 million) due to first-stage reusability. Predicting landing success helps estimate launch costs—valuable for competitors bidding against SpaceX.

While some unsuccessful landings are intentional (e.g., ocean landings), our goal is to determine whether the first stage will land successfully based on features like:

Payload mass

Orbit type

Launch site

Other mission parameters

Methodology
The project follows these key phases:

Data Collection & Preparation

Sources: SpaceX API, web scraping

Tools: Python (Requests, BeautifulSoup, Pandas)

Exploratory Data Analysis (EDA)

Libraries: Pandas, NumPy, SQL (IBM DB2)

Data Visualization

Static plots: Matplotlib, Seaborn

Interactive maps: Folium

Dashboards: Dash

Machine Learning Prediction

Algorithms: Logistic Regression, SVM, Decision Tree, KNN

Evaluation: Accuracy scores, confusion matrices

Data Collection
SpaceX API: Filtered Falcon 9 launch data (90 records, 17 features).

Web Scraping: Extracted Falcon 9 launch history from Wikipedia (121 records, 11 features).

EDA & SQL Analysis
Identified launch site distributions, orbit frequencies, and mission outcomes.

SQL queries calculated payload statistics (e.g., average mass by booster version).

Data Visualization
Matplotlib/Seaborn: Analyzed relationships (e.g., flight number vs. launch site, payload vs. success rate).

Folium: Mapped launch sites with success/failure markers.

Dash: Interactive dashboard with pie charts and scatter plots for payload vs. outcome.

Machine Learning Prediction
Data preprocessing: Standardized features, split into train/test sets.

Models tested:

Decision Tree (Best: 88.9% accuracy)

KNN (84.8%)

SVM (84.8%)

Logistic Regression (84.6%)

Discussion
Certain features (e.g., orbit type, payload mass) influence landing success. For instance:

Polar, LEO, and ISS orbits show higher success rates with heavier payloads.

GTO orbits exhibit mixed outcomes.

Machine learning helps uncover hidden patterns, enabling accurate predictions.

Conclusion
By analyzing historical Falcon 9 launch data, we built predictive models to estimate landing success—critical for cost assessment. The decision tree algorithm outperformed others, providing the most reliable predictions.

This project demonstrates how data science can optimize aerospace operations, offering competitive insights for the space industry.

(Visual examples referenced in the original text are retained as placeholders: e.g., scatter plots, Folium maps, Dash charts, and confusion matrices.)
