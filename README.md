# **Healthcare Revenue Cycle Management (RCM) Analysis**

This project focuses on **Revenue Cycle Management (RCM)** for healthcare providers. The analysis leverages hospital spending data to understand key financial metrics such as **payments**, **costs**, and **revenue gaps** across different states in the United States. The goal of this project is to provide insights into how efficiently hospitals are managing their costs and payments, as well as to identify potential areas for improvement.

## **Table of Contents**
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Analysis and Visualizations](#analysis-and-visualizations)
4. [Installation and Setup](#installation-and-setup)
5. [Usage](#usage)
6. [Results](#results)
7. [Contributing](#contributing)
8. [License](#license)

## **Project Overview**

The **Revenue Cycle Management** process is critical for healthcare organizations to maximize profitability and reduce payment delays. This project analyzes a dataset that simulates hospital costs and payments per patient. Key metrics such as **payment efficiency**, **cost efficiency**, and **revenue gaps** (the difference between payments received and costs incurred) are calculated and visualized.

### **Key Features of the Analysis:**
- **Distribution of Payments per Patient**: Understanding how payments are distributed across patients.
- **Relationship Between Payment and Cost**: Visualizing how closely aligned payments are with costs.
- **Revenue Gap Analysis**: Identifying the difference between payments and costs to assess financial health.
- **State-wise Comparison**: Analysis of how different states perform in terms of payment-to-cost ratios and revenue gaps.
- **Advanced Visualizations**: Including correlation heatmaps, payment-to-cost ratios, box plots, and more.

## **Dataset**

A simulated hospital spending dataset is used for the analysis. The dataset contains 200 records of hospital payment and cost data, including:
- `Hospital_ID`: A unique identifier for each hospital.
- `State`: The U.S. state where the hospital is located.
- `Cost_Per_Patient`: The cost incurred by the hospital per patient.
- `Payment_Per_Patient`: The payment received by the hospital per patient.
- `Revenue_Gap`: The difference between the payment and the cost for each hospital.

### **Example Record**:
| Hospital_ID | State | Cost_Per_Patient | Payment_Per_Patient | Revenue_Gap |
|-------------|-------|------------------|---------------------|-------------|
| 1           | CA    | 12,000           | 13,500              | 1,500       |

## **Analysis and Visualizations**

This analysis includes several plots and statistical summaries to better understand healthcare RCM. Below are some of the key analyses included:

### 1. **Payment Distribution:**
   - A histogram visualizes the distribution of payments across hospitals.
   
### 2. **Cost vs Payment Scatter Plot:**
   - A scatter plot shows the relationship between costs and payments for each patient, colored by state.

### 3. **Revenue Gap Calculation:**
   - The `Revenue_Gap` is calculated as `Payment_Per_Patient - Cost_Per_Patient` to assess profitability.

### 4. **State-wise Revenue Gap Analysis:**
   - Bar plots show the average and total revenue gaps by state, allowing comparison of financial performance between states.

### 5. **Advanced Plots:**
   - Box plots for payment, cost, and revenue gaps by state.
   - Heatmap for correlations between payment, cost, and revenue gaps.
   - Payment-to-Cost ratio analysis to measure efficiency.
   - Top and Bottom 5 states by revenue gap for quick identification of outliers.

### **Screenshots:**
#### Payment Distribution:
![Payment Distribution](images/payment_distribution.png)

#### Cost vs Payment Scatter Plot:
![Cost vs Payment](images/cost_vs_payment.png)

## **Installation and Setup**

### **Dependencies:**
- Python 3.7+
- Pandas
- Matplotlib
- Seaborn

### **Installation:**
1. Clone this repository:
   ```bash
   git clone https://github.com/matt7salomon/revenue_cycle_management_healthcare.git
   ```
2. Navigate to the project directory:
   ```bash
   cd revenue_cycle_management_healthcare
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## **Usage**

### Running the Jupyter Notebook:
1. Open the project in Jupyter:
   ```bash
   jupyter notebook RCM-Healthcare.ipynb
   ```
2. Run all the cells to generate the plots and analyses.

### Running the Analysis Script:
If you prefer running the script without Jupyter, you can modify and run the Python script:
```bash
python rcm_analysis.py
```

## **Results**

The analysis provides insights into the following aspects of hospital financial management:
- **Revenue Gaps**: Highlighting which states have the highest gaps between payments and costs.
- **Payment Efficiency**: Identifying states where hospitals are receiving higher payments relative to their costs.
- **Areas of Improvement**: Pinpointing states and hospitals where cost containment or payment optimization could be improved.

### Key Findings:
- **State A** shows the largest revenue gap, suggesting high profitability or overbilling.
- **State B** has the lowest payment-to-cost ratio, indicating potential financial distress or underpayment.

## **Contributing**

Contributions are welcome! Feel free to fork the repository, make improvements, and submit a pull request.

## **License**

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
