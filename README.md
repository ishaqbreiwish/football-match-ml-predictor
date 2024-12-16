### **README.md**
# Premier League Match Predictor

This project predicts the winner of football matches in the **English Premier League (EPL)** using **machine learning**.

## Project Steps
- Scrape match data using `requests`, `BeautifulSoup`, and `pandas`.
- Clean the data and prepare it for machine learning using `pandas`.
- Compute **rolling averages** of key match statistics to improve predictions.
- Make predictions about match outcomes using `scikit-learn`.

## Code Overview
- **`scraping.ipynb`**: A Jupyter notebook that scrapes and cleans match data.
- **`matches.csv`**: Processed data with rolling averages, ready for training the prediction model.
- **`prediction-model.ipnyb`**: A Jupyter notebook that preprocesses match data, and trains a random forest model on the data

## Local Setup

### Installation
To run this project locally, ensure you have the following:

- **Python 3.8+**
- **JupyterLab** or any Jupyter Notebook environment
- Required Python libraries:
   ```bash
   pip install pandas requests beautifulsoup4 scikit-learn
   ```

### Data
Match data is scraped from **FBref** using the `scraping.ipynb` notebook.  
Alternatively, you can use the provided **`matches.csv`** file if you want to skip the scraping step.

---

## Running the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/repository-name.git
   cd repository-name
   ```

2. Open the **`scraping.ipynb`** notebook in JupyterLab or Google Colab to scrape the data. Then using the resulting matches.csv file (or the one provided in this repository), open the **`scraping.ipynb`** notebook to preprocess the data, and train the model.

3. Run the notebook to:
   - Scrape the match data.
   - Clean and process the data.
   - Compute rolling averages of match statistics.
   - Train the data on a random forest model

---

## Features
- **Web Scraping**: Collect match data from FBref.
- **Rolling Averages**: Improve predictions with rolling averages of match statistics.
- **Data Cleaning**: Clean and format match statistics for machine learning.
- **Machine Learning**: Use **Random Forest** to predict match outcomes.

---

## Future Improvements
- Add player-level statistics like injuries and recent form.
- Test other ML models like **XGBoost** or neural networks for improved performance.
- Predict probabilities for **Win/Draw/Loss** instead of binary outcomes.
