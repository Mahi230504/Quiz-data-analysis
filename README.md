Please find the video here: https://drive.google.com/file/d/1uoss76HlqY2RP8SuUJsRMh2nTRBqB78X/view?usp=share_link 

Quiz Data Processing and Analysis

This project processes, analyzes, and visualizes quiz data obtained from various APIs. It includes data extraction, transformation, storage, and visualization to derive insights about quiz performance, user trends, and difficulty levels.

---

Table of Contents

1. [Features](#features)  
2. [Technologies Used](#technologies-used)  
3. [Setup Instructions](#setup-instructions)  
4. [Code Workflow](#code-workflow)  
5. [Outputs](#outputs)  
6. [Visualization Examples](#visualization-examples)  
7. [Future Enhancements](#future-enhancements)  
8. [Acknowledgements](#acknowledgements)  

---

Features

- Fetch quiz and submission data from multiple APIs.
- Process quiz metadata, including question descriptions and options.
- Calculate metrics such as:
  - Percentage scores.
  - Accuracy and negative scores.
  - Difficulty levels based on multiple weighted criteria.
- Categorize quizzes into difficulty levels: Easy, Medium, and Hard.
- Generate visualizations to:
  - Show trends in accuracy and scores.
  - Highlight weak areas across topics.
  - Compare average metrics by difficulty and topics.
- Save processed data to CSV files for further use.

---

Technologies Used

- **Python** for data processing.
- **Pandas** for data manipulation and storage.
- **Matplotlib** and **Seaborn** for data visualization.
- **Requests** for API interaction.

---

## Setup Instructions

### Prerequisites
- Python 3.x installed.
- Libraries: `requests`, `pandas`, `matplotlib`, `seaborn`.

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/quiz-data-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd quiz-data-analysis
   ```
3. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Code
1. Update the API URLs in the script with your actual endpoints.
2. Run the script:
   ```bash
   python main.py
   ```
3. View the generated CSV files and visualizations.

---

## Code Workflow

1. **Data Fetching**  
   - Fetch data from the APIs:
     - Quiz metadata.
     - Quiz submission details.
     - Data for the last 5 quizzes.
   - Handle errors and validate API responses.

2. **Data Processing**  
   - Extract key fields such as `Quiz ID`, `Question Description`, `Option Details`, and `Submission Scores`.
   - Calculate additional metrics like `Percentage Score`, `Difficulty Score`, and `Difficulty Level`.

3. **Data Export**  
   - Save processed data into CSV files:
     - `quiz_data.csv`  
     - `API_Endpoint_data_with_difficulty.csv`  
     - `quiz_submission_with_difficulty_level.csv`

4. **Visualization**  
   - Bar plots to compare scores and accuracy by difficulty level and topics.
   - Line plots to track trends over time.

---

## Outputs

- **CSV Files**  
  - **`quiz_data.csv`**: Contains detailed quiz metadata.  
  - **`API_Endpoint_data_with_difficulty.csv`**: Includes difficulty metrics for submissions.  
  - **`quiz_submission_with_difficulty_level.csv`**: Adds difficulty level categorization.

- **Visualizations**  
  - Highest percentage scores by topic.
  - Accuracy trends over submissions.
  - Quiz counts by difficulty level.

---

## Visualization Examples

1. Accuracy Over Time
![Accuracy Trend](path/to/accuracy_trend_image.png)

2. Difficulty Level Distribution
![Quiz Difficulty Distribution](path/to/difficulty_distribution_image.png)

3. Weak Areas by Topic
![Weak Areas](path/to/weak_areas_image.png)

---

Future Enhancements

- Integrate real-time data fetching using API scheduling.
- Add support for more advanced data visualizations.
- Include user authentication for personalized quiz reports.
- Support export to other formats such as Excel or JSON.

---

Acknowledgements

- JSONKeeper for API hosting.
- Seaborn and Matplotlib for visualization tools.
- Community libraries like Pandas and Requests for enabling smooth data handling.

