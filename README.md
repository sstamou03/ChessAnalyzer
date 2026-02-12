# ChessAnalyzer

## Project Description
This project predicts the outcome of chess games (White Win, Black Win, Draw) using Machine Learning. It combines traditional player ELO ratings with game quality metrics (Mean Centipawn Loss) calculated via the Stockfish chess engine. The model used is a Balanced Random Forest Classifier, selected for its ability to handle the class imbalance regarding draws.

## Data Sources and Datasets
The initial raw data was sourced from the Lichess Open Database: **lichess_db_standard_rated_2013-05**. 

* **Raw Data Link:** [https://database.lichess.org](https://database.lichess.org)

Due to its large size, the raw PGN file is not hosted in this repository. However, the repository includes the datasets at the following processed stages:
1. **Extracted Dataset:** The data after parsing moves and calculating Centipawn Loss with Stockfish.
2. **Cleaned Dataset:** The final processed dataset used for training the model.

## How to Run
1. Clone this repository or download the files.
2. Install the required Python libraries (pandas, numpy, scikit-learn, imblearn, python-chess, stockfish).
3. Open the Jupyter Notebook file.
4. **Important:** Before running the code, you must update the file paths in the `pd.read_csv()` functions to match the location where you saved the datasets on your local machine or Google Drive.
5. Run all cells to train the model and view the evaluation results.
