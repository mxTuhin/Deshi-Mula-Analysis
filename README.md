```markdown
# Company Reviews Analysis

This Jupyter Notebook analyzes company reviews from `Dataset_Of_Company_Review.csv` and generates visualizations to explore review sentiments, real vs. fake reviews, and voting patterns.

## Requirements
- Python 3.x
- Libraries: `pandas`, `matplotlib`, `seaborn`, `numpy`
- Install: `pip install pandas matplotlib seaborn numpy`

## Dataset
- File: `Dataset_Of_Company_Review.csv`
- Columns: `company`, `sentiment` (Negative, Positive, Mixed), `upvotes`, `downvotes`
- Place the file in the same directory as the notebook.

## How It Works
1. **Data Preprocessing**:
   - Removes empty sentiment reviews.
   - Converts upvotes/downvotes to integers.
   - Classifies reviews as:
     - **Real**: `upvotes > downvotes`
     - **Fake**: `upvotes <= downvotes`

2. **Charts Generated**:
   - **Chart 1**: Bar chart of Negative, Positive, Mixed sentiments for real reviews.
   - **Chart 2**: Stacked bar chart of sentiments for top 10 companies by real review count.
   - **Chart 3**: Bar chart comparing total real vs. fake reviews.
   - **Chart 4**: Bar chart of top 5 companies by score (Positive: +1, Mixed: 0, Negative: -1).
   - **Chart 5**: Bar chart of worst 5 companies by score.
   - **Chart 6a**: Stacked bar chart of sentiment breakdown for top 5 companies with most real reviews, with row-level validation.
   - **Chart 6b**: Stacked bar chart of sentiment breakdown for top 5 companies with most fake reviews, with row-level validation.
   - **Chart 7**: Grouped bar chart of upvotes and downvotes for top 10 companies by total votes.

3. **Output**:
   - Charts display inline in the notebook.
   - Saved as PNG files (e.g., `sentiment_comparison.png`, `top_5_real_reviews.png`).
   - Console prints sentiment counts and row validation for Charts 6a and 6b.

## Running the Code
1. Ensure `Dataset_Of_Company_Review.csv` is in the same directory.
2. Open `company_reviews_analysis.ipynb` in Jupyter Notebook.
3. Run all cells to generate charts and console output.

## Notes
- Colors: Negative (red, `#ff4d4d`), Positive (green, `#4caf50`), Mixed (grey, `#808080`) for Charts 6a and 6b.
- Charts 6a and 6b validate real (`upvotes > downvotes`) and fake (`upvotes <= downvotes`) reviews row-by-row.
- Adjust file path in code if dataset name/location differs.

## Dataset URL
- Kaggle: https://www.kaggle.com/datasets/aryanrahman/deshimula-dataset-9th-may-2025/data

```
