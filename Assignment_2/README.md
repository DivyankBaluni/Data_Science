# Assignment_2
## Movie Data Analysis :

### Project Overview :
This project performs data analysis on a movie dataset using Python libraries like Pandas, NumPy, Matplotlib, and Seaborn. The dataset contains information about movies such as budget, revenue, genres, language, cast, and crew.

### Technologies Used :
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

### Dataset :
- Dataset used: `imdb_data.csv`
- Contains ~3000 movie records

### Data Preprocessing :
- Removed movies with zero budget
- Created new columns:
  - **Profit** = Revenue - Budget
  - **ROI** = Profit / Budget
- Extracted:
  - **Director** from crew
  - **Producer** from crew
  - **Actors** from cast

### Analysis & Results :
#### Q1. Highest Profit Movie
- Identified the movie with maximum profit
- Extracted its director, producer, and actors

#### Q2. Language with Highest ROI
- Calculated average ROI for each language
- Found top-performing language

#### Q3. Unique Genres
- Extracted all unique genres from dataset
- Observed diversity in movie categories

#### Q4. Top Producers
- Created table of producers and directors
- Found Top 3 producers with highest average ROI

#### Q5. Most Frequent Actor
- Identified actor appearing in most movies
- Analyzed:
  - Their movies
  - Genres
  - Profit trends

#### Q6. Directors & Preferred Actors
- Selected top 3 directors
- Found actors they collaborate with most

### Visualizations :
The project includes multiple visualizations:
- **Bar Charts** (ROI, Top Movies, Producers)
- **Pie Chart** (Language Distribution)
- **Histogram** (Profit Distribution)
- **Scatter Plot** (Budget vs Revenue, ROI vs Profit)
- **Heatmap** (Correlation Analysis)

### Key Insights :
- Higher budget does not always guarantee higher profit
- Certain languages generate better ROI
- Strong collaboration exists between specific actors and directors
- Revenue has a strong correlation with profit

### How to Run :
1. Open Google Colab
2. Upload dataset:
   ```python
   from google.colab import files
   files.upload()
   ```
3. Run the notebook step-by-step
4. View outputs and visualizations

### Conclusion :
This project demonstrates how data analysis and visualization can be used to extract meaningful insights from movie datasets.

### Author :
Divyank Baluni
