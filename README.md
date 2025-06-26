# MUSIC-STREAMING-AND-LISTENERS-PREFERENCE-ANALYSIS
This report analyzes music streaming data to understand listeners' preferences, peak engagement times, artist popularity, genre trends, and market segmentation across demographics and geographies. 
![Music Streaming Analysis Dashboard screenshot](https://github.com/user-attachments/assets/9e5a31e7-3358-4a4f-9d46-dcfd1e4ddc58)
1. Introduction
With the rapid evolution of digital platforms, the music industry has undergone a transformation in how consumers access, experience, and engage with music. Streaming services have become the dominant method of music consumption, offering vast libraries accessible on-demand. This report analyzes music streaming data to understand listeners' preferences, peak engagement times, artist popularity, genre trends, and market segmentation across demographics and geographies.
1.2. Purpose of the Project
The purpose of this project is to gain actionable insights into user behavior, preferences, and engagement on music streaming platforms. By analyzing trends in streaming times, subscription models, preferred genres, and demographic interactions, stakeholders can better tailor their marketing strategies, content creation, and platform offerings to meet user demands and increase user retention.
1.3. Objectives
Identify the most played artists and top streamed music genres.
Determine peak music listening times across age demographics.
Analyze user subscription preferences (Free vs Premium).
Evaluate regional music engagement levels across different countries.
Provide strategic recommendations for content promotion, platform partnerships, and genre development.

1.4. Problem Being Addressed
There remains a gap in understanding user listening patterns, especially across varying demographics, geographic regions, and time slots. Music providers face challenges in:
Targeting appropriate content to the right audience.
Maximizing user engagement during peak times.
Promoting genre diversity and artist visibility.
Enhancing subscriber conversion and retention, especially from free to premium tiers.

This project seeks to bridge this gap with detailed analysis to drive informed decision-making and enhance user experience and business outcomes.
2.1. KEY DATASET USED
The dataset used was downloaded from Kaggle.com, a popular website for dataset. It was cleaned and analyzed to visualized the dashboard which information contained includes:
Artists' Popularity: Frequency of song plays from top artists such as Bad Bunny, Adele, Post Malone, etc.
Genre Distribution: Percentage share of music genres streamed (Reggae, Jazz, EDM, Rock, R&B).
Listening Time Trend: Distribution of total listens segmented by time of day (Night, Afternoon, Morning).
Age Demographics: Streaming frequency across age groups (10–60 years).
Subscription Types: Number of users subscribed to Premium vs Free services.
Geographic Insights: Songs rated by listeners from countries such as Australia, South Korea, UK, etc.
Platform Analysis: Usage statistics across major streaming services (Amazon Music, Tidal, Deezer, Spotify, YouTube, Apple Music).

2.2. Methodology
The methodology for this analysis included:
Data Aggregation: Collected usage statistics from various streaming services including listening hours, subscriber data, artist rankings, and geographic listening trends.
Visualization & Dashboarding: Created visual representations (bar graphs, pie charts, trend lines) to highlight key patterns and comparative insights.
Segmentation Analysis:

Temporal Segmentation: Analyzed user activity across different times of day.
Demographic Segmentation: Grouped listener data by age.
Geographic Segmentation: Compared listener ratings across countries.

Comparative Analytics:

Compared popularity across artists and genres.
Evaluated user engagement across different platforms.

Insight Generation: Interpreted visual data to generate recommendations focused on content strategy, market expansion, and platform development.

3.0 STORY OF THE DATA
3.1. Data Source
Though the data used in this report was downloaded from Kaggle.com a popular website for dataset. However, it was cleaned and compiled from multiple popular music streaming platforms, including:
Amazon Music (highlighted as the most used platform),
Tidal,
Deezer,
Spotify,
YouTube, and
Apple Music.

Additional information was sourced from user interaction logs, subscription databases, and content streaming metrics recorded through API access or internal analytics dashboards provided by these services.
3.2. Data Collection Process
The data was collected through the following mechanisms:
User Activity Logs: Tracking plays, skips, listening times, and device usage.
Platform Analytics: Aggregated statistics from music platforms on genres, artists, and peak usage.
User Profiles: Metadata associated with age, subscription type, and country (all anonymized for privacy).
Rating Systems: Country-based song ratings where users rate songs after listening.
Time-stamped Interactions: Recorded streaming behaviors across time-of-day (morning, afternoon, night).

The data collection ensured user privacy by aggregating information and avoiding the use of personally identifiable data.
3.3. Data Limitations and Biases
While the dataset offers rich insights, several limitations and biases must be acknowledged:
Platform Bias: Amazon Music shows the highest usage - this could be skewed if the dataset favors this platform due to data availability.
Time Constraint: Data may reflect only a specific period (e.g., a month or quarter), not capturing seasonal variations or long-term trends.
Regional Gaps: Not all global markets are represented equally. For example, data focuses on a handful of countries like the UK, France, Brazil, etc.
Demographic Oversimplification: Age groups are broad and may not fully reflect nuanced preferences within age brackets.
Genre Classification: Some music may overlap genres (e.g., EDM vs. Pop), potentially leading to misclassification.
User Behavior Underreporting: Passive listeners (those who don't rate or interact beyond listening) may not be fully captured.
Subscription Reporting: The sharp contrast between Premium and Free users might overlook hybrid or family plans.

4 DATA SPLITTING AND PREPROCESSING
4.1. Purpose
The main purpose of data splitting and preprocessing is to:
Ensure data quality and reliability before analysis,
Prepare the dataset for insightful visualization and modeling,
Enable fair evaluation of patterns across different user segments, and
Support decision-making with accurate, clean, and well-structured data.

Proper preprocessing eliminates noise, reduces bias, and ensures the insights derived reflect true user behavior and trends.
4.2. Data Cleaning
Data cleaning involved several steps:
Duplicate Removal: Repeated logs for the same song play were identified and eliminated.
Standardization: Artist names, genre labels, and country names were normalized (e.g., "USA" - "United States").
Outlier Detection: Extremely high play counts or ratings (possibly due to bots) were filtered to ensure realistic data.
Inconsistent Time Formats: Listening time entries were formatted uniformly (e.g., converting all timestamps to 24-hour format).

4.3. Handling Missing Values
To ensure completeness and accuracy:
Missing Age or Country Info: Records without age or country were either dropped (if minimal) or imputed using the mode or relevant cluster-based inference.
Missing Genre Tags: If genre data was absent, it was inferred using artist classification or user playlist tags.
Subscription Info: Unspecified subscription types were treated as "Unknown" or categorized as "Free" for conservative estimation.

4.4. Data Transformation
Transformation was carried out to optimize analysis:
Categorical Encoding: Genre, subscription type, and platform were encoded using label or one-hot encoding for visualization or modeling.
Aggregation: Listening data was grouped by artist, genre, and time period to compute meaningful trends (e.g., total listens per daypart).
Time-Based Segmentation: Listening timestamps were categorized into bins - Morning, Afternoon, Night - for trend analysis.
Normalization: Play counts and ratings were normalized across countries to account for population size and usage levels.

4.5. Data Splitting
For deeper analysis and testing hypotheses:
Training/Test Split: If machine learning models (e.g., recommendation engines) were built, data was split (e.g., 80/20) to train and validate predictions.
Demographic Splitting: Data was segmented by age groups (10–19, 20–29, etc.) to compare listening preferences.
Geographic Splitting: Country-level analysis allowed for insights into regional content performance.
Subscription-Based Split: Differentiating Free vs Premium users helped in understanding content engagement and monetization patterns.

4.6. Industry Context
This data preprocessing was performed within the context of:
A competitive and fast-evolving music streaming industry, where user engagement and retention are crucial.
A global audience, with diverse music preferences and consumption patterns.
A need for real-time personalization, requiring accurate data to fuel content recommendations, advertisements, and strategic decisions.

4.7. Stakeholders
Key stakeholders who benefit from the preprocessing and analysis include:
Streaming Platforms (e.g., Amazon Music, Spotify): To optimize user experience and retention strategies.
Music Labels and Artists: To understand which genres and artists are trending in specific demographics or countries.
Advertisers: To target ads based on peak listening times and demographic behaviors.
Content Curators and Playlist Managers: To create genre- or mood-based playlists based on accurate listening patterns.
Product Managers and Analysts: For insights into feature development and platform performance.

4.8. Value to the Industry
Effective data splitting and preprocessing:
Enables hyper-personalization of content and ads,
Supports data-driven decision-making for marketing, A&R (Artist and Repertoire), and platform development,
Enhances user retention by identifying key behavioral trends,
Improves revenue forecasting by understanding Premium vs Free user behaviors,
Supports geographical expansion by highlighting untapped or high-potential markets (e.g., France, Brazil).

5. PRE-ANALYSIS
5.1. Key Trends Identified
Top Music Artist: Bad Bunny leads as the most played artist with 528 plays, ahead of Post Malone and Adele.
Top Genre: Reggae and Jazz are equally the most streamed genres (20.44% each), showing a strong preference for rhythm-rich, culturally-rooted music.
Listening Time Peak: The Night is the highest listening time, with 1,745 counts, followed by Afternoon (1,634) and Morning (1,621), indicating higher engagement during off-work hours.
Subscription Dominance: The majority of users are on Premium plans (2,526) compared to Free (247), suggesting a paying audience prefers uninterrupted or exclusive content.
Popular Streaming Platforms: Amazon Music (861), Tidal (850), and Deezer (844) lead in user preference, slightly above Spotify and YouTube, with Apple Music ranking lowest.
Age Distribution: Highest engagement is seen in the 50–60 age group (1,152), followed closely by 30–39 (1,058) and 40–49 (1,047), showing mature users are more active.

5.2. Potential Correlations Identified
Premium Subscription vs Engagement: Platforms with higher premium subscribers (e.g., Amazon Music, Tidal, Deezer) have stronger user engagement, likely due to better features or exclusive content.
Age and Listening Behavior: Older demographics (50–60 years) show higher listening rates, potentially correlating with more leisure time or disposable income for premium content.
Top Genre vs Listening Time: Reggae and Jazz topping the list could correlate with relaxed, night-time listening habits, aligning with peak hours being at night.
Country Ratings vs Artist Plays: Australia and South Korea show the highest song ratings, possibly linked to the popularity of artists like BTS (South Korea) and possibly global/regional promotions.
Artist Popularity vs Platform Influence: The popularity of artists like Bad Bunny and Adele may be driving engagement on platforms like Amazon Music and Tidal, suggesting cross-promotion potential.

5.3. Initial Insights
Genre Diversification Opportunity: While Reggae and Jazz dominate, genres like EDM, Rock, and R&B also have nearly comparable shares, indicating a balanced and varied musical taste among users.
Localized Marketing Needed: France has the lowest song rating (493), indicating a potential for targeted campaigns to boost engagement and cater to regional preferences.
Strategic Time-Based Campaigns: Night hours being the most active presents an opportunity to release exclusive content, live sessions, or promotions during those periods.
Influencer and Artist Strategy: Leveraging high-performing artists (e.g., Bad Bunny, Adele, Billie Eilish) through exclusive content or collaborations could significantly enhance platform engagement and loyalty.
Platform Partnership Focus: Strengthening ties with Amazon Music, Tidal, and Deezer, which lead in user numbers and likely satisfaction, is strategic for business expansion and campaign effectiveness.

6 IN-ANALYSIS
6.1. Ongoing Observations and Unconfirmed Insights
Gender and Regional Preferences Unknown
 While Bad Bunny is the most played artist globally, it's unclear whether this preference is uniform across gender and regional lines. Gender-segmented or regional data would confirm if this trend is consistent or concentrated in specific demographics.
Peak Listening Time vs. Device Usage
 Although night is identified as the peak listening time, it's not confirmed whether this is linked to mobile, desktop, or smart speaker usage. Understanding device preferences could guide UI/UX design and marketing channel selection.
Subscription Type Impact on Listening Time
 Premium subscribers dominate user count, but it's unclear whether they contribute proportionally more to listening hours. A correlation analysis is needed between subscription type and engagement time to validate the impact of paid tiers.
Genre Popularity Driven by Algorithms or Choice?
 Reggae and Jazz lead in genre streams, but it's not clear if this is user-driven or a result of platform-curated playlists. Insight into algorithmic influence could better guide content strategies.
Low Youth Engagement (10–19)
 The 10–19 age group has the lowest music listening count (701). This could be due to:

a.  Competing platforms (e.g., TikTok, gaming).
b.  Limited access to premium services.
 But this remains unconfirmed without supporting data on user preferences or time spent on other platforms.
Underperformance of Apple Music
 Apple Music has the lowest user count (796), but the reason - pricing, content variety, or user experience - requires deeper exploration.

7. POST-ANALYSIS AND INSIGHTS
7.1. Key Findings (Confirmed Through Full Analysis)
Bad Bunny Leads Global Popularity: Confirmed as the most played artist with 528 streams, showing consistent dominance over both international and regional artists.
Reggae and Jazz Tie as Top Genres: Each commands 20.44% of total genre streams, confirming their shared popularity across platforms and user bases.
Premium Subscription Dominates Listener Base: With 2,526 premium users compared to 247 free, premium subscribers form the majority, validating monetization potential through exclusive content and ad-free experience.
Nighttime is Peak Listening Period: 1,745 streams during the night - validated as the optimal time for engagement strategies such as exclusive releases or targeted ads.
Amazon Music, Tidal, and Deezer are Top Platforms: All three platforms have over 840 users, outperforming Spotify and Apple Music, confirming earlier assumptions that they command the most loyal or satisfied user bases.

7.2 Insights Beyond Initial Expectations
Underperformance of Youth Segment (10–19): Despite being highly digital, the 10–19 age group has the lowest listening rate (701) - unexpected and suggests a possible shift toward short-form or non-traditional audio platforms (e.g., TikTok, YouTube Shorts).
EDM Nearly Matches Top Genres: At 20.28%, Electronic Dance Music trails Reggae and Jazz only slightly, highlighting an opportunity to push EDM campaigns despite it not being initially spotlighted.
Streaming Platform Competition Is Tight: Differences among top streaming platforms are marginal:

a. Amazon Music (861),
b. Tidal (850),
c. Deezer (844),
d. Spotify (827),
e. YouTube (822). This reveals an ultra-competitive landscape where platform loyalty may shift with minor user experience or content changes.
4. Even Genre Distribution: The top 5 genres all hover around 19%–20%, indicating no dominant genre monopoly. This opens up potential for curated genre-blended playlists or broader cross-genre promotions.
5. Listening Engagement Increases with Age: The trend contradicts the general expectation that younger users are more active listeners. Older age groups (30–60) are more consistent and possibly more valuable in long-term subscription retention.
 OBSERVATIONS
Music consumption is concentrated during nighttime hours, predominantly by premium users aged 30–60.
Bad Bunny, Reggae, and Jazz are market leaders across artists and genres.
Amazon Music, Tidal, and Deezer show the strongest user engagement, though Spotify and YouTube remain close competitors.
Younger audiences (10–19) are the least engaged, defying common expectations about youth digital behavior.
Country-wise, Australia, South Korea, and the UK lead in engagement metrics, while France ranks lowest, suggesting untapped potential.

RECOMMENDATIONS
Time-Specific Campaigns: Launch exclusive content, offers, or live sessions at night, when user activity peaks.
Genre Diversification Strategy: Expand investment in EDM and Rock, which show high engagement near top genres. Promote genre fusion playlists to cater to blended tastes.
Audience Retargeting for Youth (10–19): Partner with short-form content platforms like TikTok or gaming apps to re-engage the younger demographic.
Localized Marketing in France: Introduce French-language campaigns, regional artist promotions, and local playlists to boost song ratings and user engagement in underperforming countries.
Leverage Platform Loyalty: Strengthen collaborations with Amazon Music, Tidal, and Deezer for exclusive artist releases and loyalty rewards.
Premium User Monetization: Offer exclusive experiences or premium-only access with top artists like Bad Bunny and Adele to retain and upsell premium users.

CONCLUSION
The analysis confirms that user preferences are diverse, time-sensitive, and platform-specific. While top performers like Bad Bunny and Reggae stand out, even genre distribution and platform competition highlight the need for dynamic, personalized, and localized marketing strategies. Mature users show strong loyalty, while youth engagement needs innovative solutions. This positions the music streaming industry at a strategic inflection point for data-driven growth.
Key Learnings
Peak periods (night) offer the greatest return for promotions.
Genre leadership does not mean monopoly - user interests are spread across multiple genres.
Older listeners are reliable consumers, while younger groups need creative re-engagement.
Regional preferences matter - a global strategy needs local adaptations.
Platform parity means that user retention efforts must focus on value-added services.

Future Research Areas
Gender-Based Listening Patterns: To personalize recommendations and promotions more effectively.
Impact of Devices on Listening Habits: Mobile vs. desktop vs. smart speaker usage to improve app development and advertising format.
Churn and Retention Rates Across Platforms: Understand why users leave or remain on certain services to refine user experience.
Mood and Activity Tagging in Listening: Explore links between music consumption and user mood, activity, or mental state.
Podcast vs. Music Preferences: As hybrid platforms rise, understanding this split could guide future content investments.
