Spotify Analysis: What Makes a Hit.

Overview
This project analyzes why certain songs achieve high popularity on Spotify while others do not. Using a combination of exploratory data analysis, interactive dashboards, and an interpretable logistic regression model, the analysis identifies the key drivers of popularity in the modern streaming era.
The focus is not on predicting a fixed “hit formula,” but on understanding relative drivers of success within a given release period, acknowledging that music trends evolve year over year.

Objectives
•	Identify factors that differentiate popular songs from others
•	Analyze how audio features evolve over time
•	Assess the role of discovery platforms in amplifying popularity
•	Validate insights using an interpretable predictive model

Data Description
•	The dataset includes Spotify-related song metadata and performance metrics, covering releases from 2011 to 2025, such as:
•	Audio Features (e.g., BPM, danceability, energy)
•	Streaming performance
•	Discovery indicators (Spotify charts)
•	Artist-level metadata
•	Popularity is defined as songs belonging to the top 25% by average streams per year.

Methodology
Feature Engineering
•	Year-wise normalization (z-score) applied to selected audio features
•	Binary discovery indicator created using top-quartile Spotify chart presence
•	Careful handling of missing values and data integrity constraints

Exploratory Data Analysis (EDA)
•	Year-over-year trends in audio features
•	Distribution and concentration of popular songs
•	Artist-level repeat success patterns
•	Relationship between discovery exposure and popularity

Predictive Modeling
•	Logistic Regression used as an interpretable classification model
•	Purpose: validate which factors consistently differentiate popular songs
•	Inputs: Year-normalized audio features & Spotify discovery signal
•	Model performance evaluated using ROC-AUC, accuracy, and classification metrics
•	The model is designed for within-period differentiation, not forward forecasting.

Power BI Visualization Report
•	Interactive dashboards were built to support visual exploration of:
•	Year-over-year audio feature trends
•	Discovery exposure vs popularity
•	Distribution of streams across discovery buckets
•	Power BI was used strictly for insight generation and communication, not modeling.

Key Insights
•	No single “hit sound” exists; audio features shift meaningfully year over year
•	Discovery platforms play a dominant role in amplifying popularity
•	Audio characteristics contribute incrementally rather than deterministically
•	Interpretability and context are critical when modeling cultural outcomes like music

Assumptions & Limitations
•	Duplicate Song IDs across source files were removed to preserve join integrity
•	Popularity is defined using a top-quartile threshold, not an absolute benchmark
•	Analysis focuses on the 2011–2025 period to ensure relevance to streaming-era dynamics
•	Correlation-based findings indicate association and should not be interpreted as causal


Tools & Technologies
•	Python: pandas, numpy, scikit-learn
•	Power BI: dashboarding and visual analytics
•	Excel: processed output and validation

Key Takeaway
•	Song popularity on streaming platforms is shaped less by a fixed audio formula and more by evolving trends combined with platform-driven discovery and amplification.
