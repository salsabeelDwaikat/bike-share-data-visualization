# Ford GoBike System Data — Exploratory & Explanatory Data Visualization

## Overview
This project explores the **Ford GoBike bike-sharing system** (February 2019, San Francisco Bay Area) to understand rider behavior, then distills the findings into a short, polished presentation for a non-technical audience. It's split into two parts, following the standard exploratory → explanatory data visualization workflow.

- **Part I — Exploratory Analysis:** A systematic investigation of trip duration, usage timing, and rider demographics, moving from single-variable plots to multivariable relationships.
- **Part II — Explanatory Presentation:** The strongest findings from Part I, refined into a small set of clear, audience-ready slides/visuals.

## Dataset
`201902-fordgobike-tripdata.csv` — 183,412 individual bike trips, including trip duration, start/end time and station, and rider demographics (user type, birth year, gender).

## Questions Investigated
1. What is the distribution of trip durations?
2. When are bikes used most — which hours and days see peak demand?
3. How does user type (Subscriber vs. Customer) affect ride behavior?
4. What is the relationship between rider age and trip duration?
5. How do gender and user type together influence trip duration?

## Key Findings
- **Trip duration is short and right-skewed** — most rides last 5–15 minutes.
- **Weekday demand follows a clear commuter pattern**, peaking at 8 AM and 5–6 PM, while weekend demand spreads evenly across the day.
- **User type is the dominant predictor of trip duration** — Customers ride roughly twice as long as Subscribers, consistently across age, gender, and day of week.
- **The Customer/Subscriber gap widens on weekends**, consistent with Subscribers commuting and Customers riding for leisure.
- **Rider age has almost no effect on trip duration**, despite ages spanning 16–80.

Together, these point to two distinct rider populations: daily commuters on subscriptions, and casual, leisure-oriented single-ride users.

## Repository Contents
```
├── Part_I_notebook.ipynb    # Exploratory analysis: univariate → bivariate → multivariate plots
├── Part_I_notebook.html     # Rendered export of Part I
├── Part_II_notebook.ipynb   # Explanatory slide deck: final polished visualizations + narrative
├── Part_II_notebook.html    # Rendered export of Part II
└── README.md
```

## Tools Used
Python, pandas, NumPy, matplotlib, seaborn, Jupyter Notebook

## How to View
- Open the `.ipynb` files directly on GitHub to see the code and rendered charts, or
- Open the `.html` files in a browser for a clean, read-only version of each notebook.
