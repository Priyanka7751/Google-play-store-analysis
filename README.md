# Google-play-store-analysis

![Google Play Logo](https://upload.wikimedia.org/wikipedia/commons/7/78/Google_Play_Store_badge_EN.svg)

## 🧩 Problem Statement
The Google Play Store hosts millions of Android apps across various categories. With such an enormous volume of data, it's challenging for developers, marketers, and users to understand what makes an app successful. This project explores the Google Play Store dataset to analyze:

- What kind of apps receive higher ratings and reviews?
- Do free apps perform better than paid ones?
- How do categories and app size affect user perception and installs?
- What are the dominant trends in genres and content ratings?

The goal is to uncover insights that could help app developers and stakeholders optimize their product offerings and marketing strategies.

## 📂 Dataset Overview
- **Source:** [Kaggle - Google Play Store Dataset](https://www.kaggle.com/datasets/lava18/google-play-store-apps)
- **Total Records:** 10,000+ apps
- **Features:**
  - App Name, Category, Rating, Reviews, Size, Installs, Type (Free/Paid), Price, Content Rating, Genres, Last Updated, Current Version, Android Version

## Features
**App Category**: Category of the app. This could be beauty, business, entertainment, education...etc.
**Rating:** How users rate the app out of 5, with 1 being the lowest rating and 5 being the highest.
**Reviews:** The number of user reviews each app has received.
**Size:** The memory size needed to install the application.
**Installs:** The number of times each application has been installed by users.
**Type:** Whether the app is free or a paid app.
**Price:** The price of the app.
**Content Rating:** This column specifies the intended audience for the app. Can be for teens, mature audience, or everyone.
**Genres:** The sub-category for each app. Example: for the Education category, this could be Education: Pretend Play, for example.
**Last Updated:** Release date of the most recent update for the app.
**Current Ver:** The app's current version.
**Android Ver:** The oldest version of Android OS supported by the app.

## 🛠️ Tools and Technologies Used

- Python
- Jupyter Notebook
- Pandas & NumPy
- Matplotlib & Seaborn
- Regular Expressions
- Feature Engineering
- Data Cleaning & EDA

## 🧹 Data Cleaning & Preprocessing

✔ Filled missing ratings using column mean  
✔ Dropped rows with critical null values (e.g., Current Version, Android Version)  
✔ Converted `Size` to megabytes, removed `Varies with device`  
✔ Cleaned `Installs` and `Price` columns (removed `+`, `,`, `$`, and converted to numeric)  
✔ Created new feature: `Installs_Category` using custom bins  
✔ Unified values in `Content Rating`  
✔ Simplified `Genres` to retain the primary genre only  
✔ Reset index and adjusted data types

## 📊 Exploratory Data Analysis (EDA)

We explored the data through the following key questions:

1. Correlation between numerical variables
2. Average rating by genre
3. Free vs Paid app performance comparison
4. Average size and rating by install category
5. Most common app categories
6. Categories with the most installs, reviews, and ratings
7. Most expensive apps
8. Distribution of ratings
9. Distribution of free vs paid apps
10. Top 10 genres by app count and total installs
11. Correlation between app size and ratings
12. Correlation between price and ratings
13. Content Rating-wise app distribution and installs

## 📈 Key Visualizations

- Distribution plots of Ratings.
- Barchart showing top 10 genres.
- Bar charts for Install Categories and App Categories.
- Heatmap showing correlation between numeric features
- Pie charts showing distribution of free vs paid apps.

## 💡 Key Insights

- **Free apps dominate** the Play Store, both in quantity and downloads.
- **Game, Tools, and Communication apps** have the highest install counts.
- **Paid apps are less frequent** and don’t always yield higher ratings.
- Apps targeted to **“Everyone” and “Teen”** have higher user engagement.
- **Entertainment and Education genres** show a balanced performance between installs and ratings.
- No strong correlation between app **price and ratings**.

Feel free to explore the repository to gain further insights into the code implementation, methodology, and findings.
