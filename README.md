☕️ Does Caffeine Really Boost Productivity? Building a "Caffeine & Focus" Analytics Dashboard in Power BI

Introduction:
As someone who frequently needs to deliver high-output work, grabbing "one more cup of coffee" is often my instinctive reaction to an afternoon slump. However, is the relationship between caffeine intake and focus truly linear—the more you drink, the more focused you become? To test this hypothesis, I tracked my daily caffeine intake, sleep hours, and focus scores, and built an interactive Power BI dashboard to uncover the truth behind the data.

📌 Project Summary & Core Questions
This project aims to explore three core questions through data:

Time Trends: Do focus levels follow a specific circadian pattern throughout the day?

Dose-Response: Does focus scale linearly with caffeine intake, or is there an optimal threshold?

Beverage Efficacy: Among Americano, Latte, Espresso, and Green Tea, which drink delivers the highest focus performance?

📊 Dashboard Architecture & Data Insights
1. Core KPIs: Tracking Baseline Health & Total Intake
At the top of the dashboard, I placed two core KPI cards to establish a baseline for my overall condition:

Average Daily Sleep Hours: Monitors whether my foundational physiological rest is sufficient.

Average Daily Caffeine Intake: Tracks total daily concentration to prevent over-reliance.

💡 Key Finding: When average daily sleep stays at a healthy level, caffeine's cognitive boost increases significantly. Conversely, when sleep-deprived, blindly increasing caffeine intake fails to proportionally raise focus scores.

2. Time Trend Analysis: Confirming the "Circadian Slump"
Analyzing focus across time blocks (Morning → Late Morning → Afternoon → Late Afternoon) via a line chart revealed a classic physiological curve:

Morning to Late Morning (09:00–12:00): Focus remains steadily high between 7.0 and 7.3.

Afternoon Slump (13:00–16:00): A pronounced "post-lunch dip" occurs, dropping focus to its lowest point of the day (~6.4 / 10).

Late Afternoon Rebound (After 16:00): Focus surges back up, reaching the highest peak of the day (nearly 7.8 / 10).

3. Scatter Plot Exploration: The "Inverted-U" Relationship
Plotting individual intake records on a scatter plot confirmed the psychological Yerkes-Dodson Law (moderate stimulation yields peak performance):

The Golden Zone (50–75 mg): Focus scores consistently peak above 8.0.

Diminishing Returns (> 80 mg): When a single dose is too high, focus scores actually drop, accompanied by restlessness and anxiety.

4. Beverage Comparison: Which Caffeine Carrier Works Best?
Average focus performance across different drink types:

🥇 Americano: Ranked first with the highest focus score at 7.30.

🥈 Green Tea: Followed closely at 7.25, proving that milder teas containing L-theanine are also an excellent option.

🥉 None (No Caffeine): Maintained a steady baseline of 7.00.

📉 Espresso: Scored only 6.17, reinforcing that spiking caffeine concentration rapidly often backfires.

💡 Actionable Insights & Personal Optimization Strategy
Based on the findings from this dashboard, I established three "High-Focus Caffeine Rules" for myself:

Adopt a "Micro-Dosing" Strategy: Keep single intakes within the 50–75 mg range (such as a medium Americano or Green Tea), avoiding high-concentration Espresso shots for a quick pick-me-up.

Target the Afternoon Slump Precisely: Skip caffeine right after waking up when its effectiveness is lower, and instead take a light dose around 13:00–14:00 just before the afternoon dip hits to smooth out the trough.

Dynamic Scenario Management: Using the Day_Type slicer on the dashboard to separate Workdays vs. Weekends, I deliberately scale back intake on weekends to preserve my body's sensitivity to caffeine.

🛠️ Power BI Technical Stack Used
Data Cleaning & Custom Sorting: Created a custom Time_Period_Order column paired with Sort by Column to fix chronological text sorting on the time axis.

Dynamic Data Modeling: Used DAX to calculate averages and ratio metrics, paired with Slicers for full-page cross-filtering.

Information Architecture: Combined KPI cards, time-series line charts, scatter plots, and clustered column charts to create a cohesive Data Storytelling layout.

Conclusion:
The most fascinating part of data analysis is turning intuition and assumptions into verifiable, concrete insights. Not only did this project help me optimize my daily work performance, but it also served as a complete end-to-end Power BI practice build. If you're interested in the data modeling approach or DAX formulas behind this project, feel free to leave a comment below and connect!
