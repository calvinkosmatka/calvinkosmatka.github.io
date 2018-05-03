---
layout: post
title: Visualizing Wage and Hour Compliance Actions
---

[View Here](https://calvinkosmatka.github.io/dol-whd/)

[Source](https://github.com/calvinkosmatka/dol-whd)

This is a work in progress.

The dataset used in this visualization is the Wage and Hour Compliance Action Data from the United States Department of Labor's [Enforcement Data Catalog](https://enforcedata.dol.gov/views/data_catalogs.php). It provides the names and locations of businesses investigated by the DoL, details about what wage and hour violations, if any, were found, and how those violations were remedied.

This dataset contains more than 250,000 rows (106 MB!), so I used Python and Pandas to aggregate by state and industry, reducing it to a much more manageable 28,000 rows (2 MB). The visualization itself uses D3.js and Vue.js to handle displaying and interacting with the data.

The main purpose of this visualization is to give a sense of the relative scale of wage and hour violations between states and industries.

Right now, the only purpose of the color of the dots is to make the chart more visually appealing.

One limitation of this dataset is that it only supplies ranges of dates for violations. This makes it impossible to derive exactly how many wage and hour violations occured within a specific period of time. Many of the cases in this dataset have findings dates spanning about two years. For this reason, I have not yet incorporated time into this visualization.
