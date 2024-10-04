
# Fortune 1000 Companies by HDI

## Project Overview

This project explores the relationship between the concentration and performance of the top 1000 American companies and the **Human Development Index (HDI)** of U.S. states. We aimed to investigate whether the presence and performance of top companies in a state correlate with higher HDI scores, which are indicators of overall well-being including life expectancy, education, and per capita income.

### Authors:
- Rafael Coelho
- Gunay Azizova

### Datasets:
- **Dataset 1**: Fortune 1000, 2023 ([Kaggle Dataset](https://www.kaggle.com/))
- **Dataset 2**: HDI of U.S. States, 2022 (Web Scraping from Wikipedia)

### Hypotheses:
- **H0**: States with a higher concentration of top companies exhibit a **negative** correlation with HDI scores.
- **H1**: States with a high concentration of companies in key sectors (Health, Services, Finance) exhibit a **positive** correlation with HDI.
- **H2**: States with the highest revenue-generating Fortune 1000 companies show a **positive** correlation with their HDI.

---

## Project Workflow

### Data Cleaning & Wrangling:
1. **Cleaning Dataset 1 (Fortune 1000)**: Renaming columns, filling null values, formatting, and ensuring consistency.
2. **Web Scraping for Dataset 2 (HDI)**: Extracting and formatting the HDI data from Wikipedia using Python and Pandas.
3. **Merging Datasets**: Combined the cleaned datasets into a master dataset for analysis.
4. **Data Export**: Exported the final merged dataset to Excel for further analysis and visualization.

### Visualization:
- **Tool Used**: Tableau
- **Charts and Dashboards**: Key data trends were visualized in Tableau, including company concentration by state, sectoral impacts, and revenue vs. HDI correlations.
- **Public Dashboard**: Visualizations were published to Tableau Public for wider access and review.

---

## Key Findings:

### H0: Company Concentration vs. HDI
- **Result**: No clear correlation between states with the highest concentration of Fortune 1000 companies and HDI.
- **Conclusion**: **H0 is FALSE**. States like California, Texas, and New York ranked neutrally in HDI despite their high company concentration.

### H1: Impact of Top Sectors on HDI
- **Result**: States with companies in top sectors (Health, Services, Finance) ranked higher in HDI.
- **Conclusion**: **H1 is TRUE**. States with a high concentration in these sectors showed a positive correlation with higher HDI scores.

### H2: Company Revenue vs. HDI
- **Result**: No strong correlation between states with top revenue-generating companies and HDI.
- **Conclusion**: **H2 is FALSE**. High-revenue states like Texas and California did not rank proportionately higher in HDI.

---

## Project Structure

1. **Data Selection** → 2. **Data Processing** → 3. **Analysis** → 4. **Visualization**

The project was structured to ensure that each phase was completed before moving to the next. This ensured minimal data issues and alignment across the team. We also actively used GitHub for collaboration, ensuring smooth integration of each team member's contributions and avoiding merge conflicts.

---

## Challenges & Solutions:

### Web Scraping:
- **Challenge**: Handling complex table structures with alternating row spans during web scraping.
- **Solution**: Utilized Pandas' `read_html()` method to efficiently parse and clean data from Wikipedia tables.

### Visualization:
- **Challenge**: Balancing clarity and depth in Tableau visualizations to ensure insights were easily interpretable.
- **Solution**: Created interactive dashboards that allowed viewers to drill down into specific data points.

---

## Conclusion & Insights

- **Top states by HDI**: States with companies in key sectors such as health, services, and finance tend to have higher HDI scores.
- **Revenue and HDI disconnect**: States with the highest revenue-generating Fortune 1000 companies do not necessarily rank highest in HDI, suggesting that corporate financial success does not always translate into broader human development outcomes.

---

## How to Run the Project

1. **Data Files**: Ensure you have access to the Fortune 1000 dataset from Kaggle and HDI data from Wikipedia.
2. **Python Environment**: Install the necessary libraries such as `pandas`, `requests`, `BeautifulSoup`, and `matplotlib` for data cleaning and wrangling.
3. **Tableau**: Use Tableau for visualization by connecting it to the cleaned data in Excel.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
