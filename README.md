# LEGO Set Explorer

> An interactive Power BI dashboard that helps users explore, filter, compare, and discover LEGO sets based on price, age, theme, pieces, and other characteristics.

---

## 🎥 Project Demo

**LEGO Set Explorer — Dashboard Demo**



https://github.com/user-attachments/assets/bd914e9f-deab-478d-8bec-8f37154f2a2d





## 📖 Overview

LEGO Set Explorer is an interactive Power BI dashboard designed to help users explore LEGO sets and narrow down their choices based on their preferences.

The dashboard allows users to filter and compare LEGO sets using factors such as theme group, theme, recommended age range, and price. Users can also explore detailed information about individual sets, including their price, release year, number of pieces, recommended age, and image.

The project combines ETL, data transformation, DAX, data modeling, visualization, and Power BI interactive features to convert raw LEGO set data into a user-focused exploration tool.

---

##  Problem Statement

LEGO has a large number of sets covering different themes, categories, age ranges, prices, and piece counts. With many options available, users may find it difficult to narrow down the sets that match their preferences.

The objective of this project is to transform the raw LEGO dataset into an interactive analytical dashboard that allows users to quickly filter, explore, compare, and inspect LEGO sets before deciding which sets they may prefer.

---

##  Dataset

### Source

**Maven Analytics — LEGO Set Explorer**

The dataset contains LEGO sets released between **1970 and 2022**.

It is a single-table dataset containing **18,459 records and 14 fields**.

### Key Fields

- `set_id` — LEGO set identifier
- `name` — Name of the LEGO set
- `year` — Release year
- `theme` — LEGO theme
- `subtheme` — Subtheme
- `themeGroup` — Theme group
- `category` — Set category
- `pieces` — Number of pieces
- `minifigs` — Number of minifigures
- `agerange_min` — Minimum recommended age
- `US_retailPrice` — US retail price
- `bricksetURL` — Brickset reference URL
- `thumbnailURL` — Thumbnail image URL
- `imageURL` — Full-size image URL

### Data Preparation

The dataset was prepared before analysis by:

- Removing unnecessary fields
- Reviewing and correcting data types
- Filtering records with missing price, age, pieces, or image information
- Creating new analytical categories
- Preparing the dataset for interactive filtering and visualization

---

##  Tools and Technologies

### Core Tool

- **Microsoft Power BI**

### Power BI Features and Techniques

- Power Query
- DAX
- ETL
- Data Cleaning
- Data Transformation
- Data Profiling
- Data Modeling
- Data Visualization
- Dashboard Development
- Calculated Columns
- Conditional Columns
- Measures
- Parameters
- Slicers
- Filters
- Tooltips
- Bookmarks
- Buttons
- Button States
- Page Navigation
- Visual Interactions
- Conditional Formatting
- Decomposition Tree

---

##  Methods

### 1. Data Loading and ETL

The raw LEGO dataset was imported into Power BI and prepared using Power Query.

The ETL process included:

- Loading the LEGO Sets CSV file
- Reviewing the dataset structure
- Correcting data types
- Removing unnecessary columns
- Handling missing values
- Preparing the dataset for analysis

### 2. Feature Engineering

Two conditional columns were created to make the dataset easier to analyze.

#### Age Range

| Minimum Age | Age Range |
|---|---|
| 18+ | Over 18 |
| 10–17 | 10 to 17 |
| 5–9 | 5 to 9 |
| 1–4 | 1 to 4 |

#### Price Range

| Price | Price Range |
|---|---|
| > $500 | $$$$$ |
| > $100 | $$$$ |
| > $50 | $$$ |
| > $25 | $$ |
| ≤ $25 | $ |

### 3. DAX Measures

DAX measures were created for the main analytical metrics:

- Total Sets
- Total Groups
- Average Age
- Average Price
- Average Pieces

These measures respond dynamically to user selections and filters.

### 4. Dashboard Design

The report was designed around the goal of allowing users to discover and compare LEGO sets.

The main dashboard includes:

- KPI cards
- Slicers
- Filters
- Set comparison table
- Set detail section
- LEGO set images
- Price range information
- Interactive controls

### 5. Interactive Analysis

Several Power BI features were implemented to make the dashboard interactive:

- Theme Group filtering
- Theme filtering
- Age Range filtering
- Maximum Price parameter
- Image tooltips
- Bookmark-based filter reset
- Button actions
- Page navigation
- Visual interaction controls

### 6. Decomposition Tree Analysis

A separate report page was created using the **Decomposition Tree** visual.

Users can explore the number of LEGO sets through the hierarchy:

**Category → Theme Group → Theme → Name**

This provides a drill-down view of the structure and distribution of LEGO sets.

---

## 🔍 Key Insights

The dashboard enables users to explore LEGO sets through multiple dimensions rather than relying on a single metric.

### User Exploration

Users can:

- Narrow down LEGO sets according to their preferred theme group and theme.
- Filter sets according to recommended age range.
- Set a maximum price based on their budget.
- Compare available sets using pieces, price, age, and other characteristics.
- Inspect detailed information for an individual LEGO set.
- View the corresponding LEGO set image through interactive tooltips.

### Hierarchical Exploration

The Decomposition Tree allows users to move from broader LEGO categories into specific theme groups, themes, and individual set names.

This makes it easier to explore how the LEGO collection is structured across different levels.

---

## 📊 Dashboard / Model / Output

### Main Dashboard

The main dashboard provides the primary user interface for LEGO set exploration.

<img width="1419" height="798" alt="Screenshot 2026-09-22 232939" src="https://github.com/user-attachments/assets/7f1ff3fc-2798-4e21-84e5-6d991cb01bc9" />

---

### LEGO Set Details

The dashboard includes a dedicated area for viewing information about a selected LEGO set.

<img width="524" height="522" alt="Screenshot 2026-09-22 233212" src="https://github.com/user-attachments/assets/30e4194f-55fe-48bc-baf3-25aa63a64901" />
---

### Decomposition Tree

The second report page provides hierarchical analysis using the Decomposition Tree.

<img width="770" height="569" alt="Screenshot 2026-09-22 233343" src="https://github.com/user-attachments/assets/dffc0276-4d43-490b-a446-24afcfc392bb" />
---

---

## ▶️ How to Run This Project?

### Step 1 — Download the Repository

Download or clone this repository to your local system.

### Step 2 — Open the Power BI File

Go to the:



### Step 3 — Verify the Dataset Path

The source dataset is available in:


If Power BI asks for the source file location, select the dataset stored in this folder.

### Step 4 — Refresh the Data

Refresh the dataset in Power BI if required.

### Step 5 — Explore the Dashboard

Use the report pages, slicers, filters, buttons, tooltips, and other interactive features to explore the LEGO sets.

---

##  Results & Conclusion

The project transforms raw LEGO set data into an interactive Power BI dashboard focused on user exploration and decision-making.

The dashboard allows users to:

- Explore a large collection of LEGO sets
- Filter sets according to different preferences
- Compare important set characteristics
- View detailed information about selected sets
- Explore LEGO set distributions through a Decomposition Tree
- Navigate between different report views using interactive controls

The project demonstrates an end-to-end Power BI workflow covering **ETL, data preparation, data transformation, DAX, data modeling, visualization, and interactive dashboard development**.

---

## 🚀 Future Work

Possible future improvements include:

- Adding a recommendation or scoring system based on user preferences
- Adding more user preference criteria
- Including LEGO set ratings or popularity data
- Adding newer LEGO releases as the dataset is updated
- Creating a more advanced recommendation experience based on multiple user inputs
- Developing additional analytical pages for deeper LEGO trend analysis

---

## 👤 Author & Contact

**Anant Sharma**

Aspiring Data Analyst | Power BI | Data Analytics

GitHub: [@sharmaanant491-ctrl](https://github.com/sharmaanant491-ctrl)
Mail: sharmaanant491@gmail.com
For project-related questions or feedback, please use GitHub.

---

## 📚 Sources

### Dataset

**Maven Analytics — LEGO Set Explorer**

[LEGO Set Explorer](https://mavenanalytics.io/guided-projects/lego-set-explorer)

### Design Assets

Some LEGO-themed visual assets used in the dashboard, including decorative elements, buttons, and background/design components, were sourced from:

**Magnific — LEGO Brick Design Vectors**

[LEGO Brick Design Vectors](https://www.magnific.com/vectors/lego-brick-design)
