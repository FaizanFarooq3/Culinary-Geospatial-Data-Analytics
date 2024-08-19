
# Culinary-Geospatial-Data-Analysis

## Project Summary

This project focuses on analyzing restaurant data from Zomato to provide insights into restaurant trends, costs, and cuisine preferences across Bengaluru. The goal is to help new and existing restaurants optimize their offerings by understanding the factors influencing the success of restaurants in different areas.

## Objective

The primary objective of this project is to analyze the Zomato dataset to understand the factors that influence the establishment of different types of restaurants in various locations across Bengaluru. By analyzing demographic data, the project aims to help new restaurants decide on their themes, menus, cuisines, and price ranges based on the neighborhood.

## Problem Statement

This project explores the following aspects:
1. Top restaurant chains in Bengaluru
2. Price differences between restaurants that accept online orders and those that do not
3. Availability of table reservations in restaurants
4. Types of restaurants in various areas
5. Top-rated restaurants
6. Restaurants by location in Bengaluru
7. Cost for 2 people in different areas
8. Votes for restaurants that accept online orders vs those that don’t
9. The most expensive restaurant and its signature dish
10. Top 10 most expensive and cheapest restaurants for two people
11. Budget hotels under ₹500
12. Budget-friendly restaurants with ratings above 4
13. Total restaurants rated above 4 and costing less than ₹500
14. Affordable restaurants in different neighborhoods
15. Popular food spots
16. Heatmap of North Indian and South Indian restaurants
17. Most popular casual dining chains
18. Favorite dishes represented via word clouds

## Installation and Setup

### Dependencies
- Python 3.x
- Jupyter Notebook
- Required libraries:
    - pandas
    - numpy
    - plotly
    - seaborn
    - matplotlib

### Installation Guide
1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd Culinary-Geospatial-Data-Analysis
    ```
2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```
3. Launch the Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

### Environment Setup
- No specific environment variables are required.

## Usage Instructions

To run the analysis, open the Jupyter Notebook and follow the cells step by step.

Here are some example usages:

### Running Analysis
```python
# Example: Load the dataset and generate a scatterplot of restaurant ratings
import pandas as pd
import seaborn as sns

df = pd.read_csv("zomato.csv")
sns.scatterplot(data=df, x="average_cost_for_two", y="rating")
```

### Sample Outputs

- **Heatmap Example:**
    ![Heatmap Example](images/heatmap.png)

- **Word Cloud Example:**
    ![Word Cloud Example](images/wordcloud.png)

## Data Sources

The analysis is based on the following dataset from Zomato. 

- [Zomato Bengaluru Dataset](<dataset-link>)

### Data Preparation

The data was cleaned and preprocessed to remove missing values, handle duplicates, and transform categorical variables into a usable format for analysis.

## Technical Details

### Methodology
This project uses a variety of analytical methods, including clustering, regression analysis, and heatmap generation, to explore the relationships between restaurant types, costs, ratings, and location data. These methods were chosen to gain a deeper understanding of how demographic factors affect restaurant success.

### Tools and Libraries

- **Jupyter Notebook**: Used as the primary IDE for developing and documenting the analysis.
- **Pandas and NumPy**: Used for data cleaning, preprocessing, and manipulation.
- **Plotly, Seaborn, Matplotlib**: Visualization libraries used to create interactive and static plots to better understand the data.

## Architecture Diagram

Below is a simple architecture diagram illustrating the flow of the analysis:

```plaintext
[Zomato Dataset] --> [Data Preprocessing] --> [Analysis Methods: Clustering, Heatmaps] --> [Visualizations]
```

## Results and Insights

- **Top Restaurant Chains**: Cafe Coffee Day dominates the landscape followed by Onesta and Empire.
- **Online Orders**: 64.4% of restaurants accept online orders.
- **Cuisine Trends**: North Indian, Chinese, and South Indian are the most common cuisines.
- **Affordable Restaurants**: The majority of restaurants in Bengaluru are priced under ₹1000.
- **Restaurant Hotspots**: BTM, HSR, and Koramangala 5th Block have the highest density of restaurants.

## Contributing

Contributions are welcome! Please follow the guidelines below:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a Pull Request.

Please ensure that your code adheres to our coding standards and includes relevant tests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## FAQ

1. **Can I use this project for commercial purposes?**
    - Yes, the project is licensed under MIT, which allows for commercial use.

2. **How can I contribute?**
    - Follow the contribution guidelines outlined above.

## Acknowledgments

Special thanks to the Zomato team for providing the dataset and to all contributors who helped in developing this project.
