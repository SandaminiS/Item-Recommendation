# STA6714: Assignment - Online Retail

## Overview
This project is part of my final assignment for STA6714 and aims to develop a model that recommends additional items to customers based on their current orders. The primary goal is to encourage customers to add a relevant item to their invoice, enhancing their shopping experience and increasing average order value.

## Project Goals
- **Recommendation Objective**: Create a model that considers which items are currently being ordered and recommends an item that is not on the invoice.
  
## Dataset Information
- **Dataset Source**: The data set used for this project is the Online Retail dataset from the UCI Machine Learning Repository. 
- **Download Link**: [Online Retail.xlsx](https://archive.ics.uci.edu/ml/datasets/online+retail)

## Deliverables
The following datasets was submitted as part of the assignment:

### Recommendation Data Set
- This dataset contains two columns:
  - **Invoice Number**: The unique identifier for each invoice (first column).
  - **Recommended Item Description**: The description of the recommended item as it appears in the original data (second column).
  
  Each invoice will appear once in this dataset, and the recommended item must not be included in the original invoice.

### Summary Table
- The summary table will include three columns:
  - **Recommended Item Description**: The description of the recommended item as it appears in the original data (first column).
  - **Count of Item Appearances**: The total number of times the item appears in invoices (second column).
  - **Count of Recommendations**: The total number of times the model recommended the item (third column).

## Data Preparation
To build an effective model, several key considerations will be addressed:
- **Grouping Similar Items**: Due to the high number of distinct items for purchase, similar items will be grouped together before modeling, ensuring that only one item is recommended per invoice.
- **Reshaping Data**: The original data is in long format (item by invoice). The data will be reshaped into wide format, where each invoice corresponds to a single row.
- **Efficient Data Processing**: With over half a million rows in the dataset, effective data preparation and computational efficiency will be crucial for modeling.

## Implementation Steps
1. **Data Loading**: Import the dataset and review its structure.
2. **Data Cleaning**: Address missing values, duplicates, and irrelevant records.
3. **Data Reshaping**: Transform the dataset from long format to wide format for analysis.
4. **Model Development**: Implement the recommendation model based on grouped items and customer purchase behavior.
5. **Output Generation**: Create the recommendation dataset and summary table as specified.

## Future Enhancements
- **Advanced Recommendation Techniques**: Explore collaborative filtering and machine learning approaches for more sophisticated recommendations.
- **Customer Feedback Analysis**: Incorporate customer feedback to refine and enhance the recommendation process.

## Getting Started
To run this project locally, please follow these steps:
1. Clone the repository: `git clone <repository_url>`
2. Install the necessary dependencies: `pip install -r requirements.txt`
3. Run the data preparation and modeling scripts: `python model.py`
4. Access the results in the output directory.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- This project was developed as a final assignment for STA6714.
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/online+retail) for providing the dataset.
