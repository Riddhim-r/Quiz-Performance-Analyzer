# AI-Powered Quiz Performance Analysis

## Project Overview

This project analyzes quiz performance using AI to provide personalized feedback and recommendations based on quiz scores and accuracy. It combines real-time quiz data and historical performance to generate insights, visualize trends, and produce recommendations for improvement.

## Approach

1. **Data Collection**:        
   - The project fetches real-time quiz data and historical performance data from APIs.
   - Data includes quiz scores and accuracy percentages for both current and historical submissions.

2. **Data Processing**:
   - The project analyzes both datasets to calculate average scores and accuracies.
   - A performance comparison is made between current quiz data and historical quiz data.

3. **Visualization**:
   - Data visualizations are created using bar charts to compare average scores and accuracies.

4. **Recommendations**:
   - Based on performance thresholds, the system provides recommendations for improvement.

5. **PDF Report Generation**:
   - A personalized PDF report is generated with insights and recommendations.

6. **File Downloads**:
   - The PDF report is downloadable for users to review their performance.

## Setup Instructions

### Prerequisites
- Python 3.x
- Required Libraries:
  - `requests`
  - `matplotlib`
  - `reportlab`
  
### Libraries
The following libraries are required to run the project:

- `requests` - For fetching data from external APIs
- `matplotlib` - For data visualization
- `reportlab` - For generating PDF reports

To install the necessary libraries, you can use `pip`:

```bash
pip install requests matplotlib reportlab
```

### JSON Files

You will need to download the following JSON files to use the project:

1.  **Current Quiz Data - Quiz Endpoint Data**: [Link](https://jsonkeeper.com/b/LLQT)
2.  **Current Quiz Data - Quiz Submission Data**: [Link](https://api.jsonserve.com/rJvd7g)
3.  **Historical Quiz Data**: [Link](https://api.jsonserve.com/XgAgFJ)

### Running the Project

1.  Clone this repository:
    
    ```bash
    git clone https://github.com/yourusername/quiz-performance-analysis-ai.git
    cd quiz-performance-analysis-ai
    ```

2.  Ensure you have the downloaded JSON files (from the links above) placed in the project directory.
    
3.  Run the Python scripts:
    
    *   To fetch and analyze quiz data:
        
        ```bash
        python fetch_and_analyze.py
        ```
        
    *   To generate the PDF report:
        
        ```bash
        python generate_pdf_report.py
        ```
        
4.  The script will generate a `Quiz_Performance_Report.pdf` that you can view or download.
