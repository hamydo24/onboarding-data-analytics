1. What are the advantages of using Pandas for data manipulation?
Pandas is a powerful library for working with structured data. Its advantages include:

Easy data loading from CSV, Excel, SQL, and more

Intuitive syntax using DataFrame and Series objects

Rich data manipulation tools: filtering, sorting, grouping, merging, reshaping

Built-in time series support for date/time-indexed data

Strong integration with visualization (Matplotlib, Seaborn) and analysis libraries (NumPy, Scikit-learn)

Pandas helps analysts focus on insight generation rather than low-level data wrangling.

2. How do you filter and aggregate data in Pandas?
Filtering
You can filter rows using conditions:

python
Sao chép
Chỉnh sửa
# Filter users who completed a task
df[df['task_completed'] == True]

# Filter by date range
df[(df['date'] >= '2024-01-01') & (df['date'] <= '2024-01-31')]
Aggregation
Use groupby() to aggregate data:

python
Sao chép
Chỉnh sửa
# Average session duration per user
df.groupby('user_id')['session_duration'].mean()

# Total sessions per day
df.groupby('date').size()

# Multiple aggregations
df.groupby('feature_used').agg({
    'session_duration': 'mean',
    'user_id': 'nunique'
})
These techniques are essential for extracting summaries and trends.

3. What techniques help handle missing or incorrect data?
Pandas provides flexible tools to clean and validate data:

Detect missing values: df.isnull(), df.isna()

Drop missing rows/columns: df.dropna()

Fill missing values: df.fillna(value), df.fillna(method='ffill')

Replace incorrect values: df.replace(old, new)

Type conversion and validation: df.astype(), pd.to_datetime(), custom assertions

Example:

python
Sao chép
Chỉnh sửa
# Fill missing task status with 'incomplete'
df['task_status'] = df['task_status'].fillna('incomplete')
4. How would Pandas be useful for analyzing Focus Bear’s user activity data?
Pandas would enable the Focus Bear team to:

Track user behavior
Load event logs and filter by feature, session duration, or completion status.

Segment users
Group by user type, activity level, or onboarding date for deeper analysis.

Monitor engagement over time
Aggregate events daily or weekly to see usage trends.

Analyze feature adoption
Count how many users tried new features and their impact on retention.

Identify churn risks
Detect inactive users and calculate time since last activity.

Generate reports
Summarize key metrics (e.g., average daily usage) for stakeholders.

By combining these with visualizations, Pandas makes large datasets easy to understand and act upon.