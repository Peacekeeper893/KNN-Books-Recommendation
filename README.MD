# KNN Books Recommendation System

This project implements a K-Nearest Neighbors (KNN) based recommendation system for books using the Goodreads dataset. The system recommends books based on user ratings and book popularity.


- `goodreads_books.csv`: Contains information about books.
- `goodreads_ratings.csv`: Contains user ratings for books.
- `output/`: Directory containing the trained KNN model and the processed data.
  - `model_knn.pkl`: Trained KNN model.
  - `rating_popular_book.csv`: Processed data with popular books.
- `README.MD`: This readme file.
- `test.ipynb`: Jupyter notebook for testing the recommendation system.
- `train.ipynb`: Jupyter notebook for training the recommendation system.

*The dataset can be found [here](https://drive.google.com/drive/folders/1qo-uUPkys5z-6KKF4cyZ1QRXDieQmvkX?usp=sharing)*

## Setup

1. Clone the repository.
2. Install the required Python packages:
   ```sh
   pip install pandas numpy scikit-learn

   ```

3.  **Training the Model** :
    - Open train.ipynb in Jupyter Notebook.
    - Run all cells to preprocess the data and train the KNN model.
    - The trained model will be saved as output/model_knn.pkl.
4. **Testing the Model:**
    - Open test.ipynb in Jupyter Notebook.
    - Run all cells to load the trained model and test the recommendation system.
    - Enter the name of a book to get recommendations.

## Example

After running the `test.ipynb` notebook, you might see output like this:

```python
You have entered:  The Handmaid's Tale
```

```
Recommendations for The Handmaid's Tale:

1: 1984, with distance of 0.6362589552000611:
2: Memoirs of a Geisha, with distance of 0.6452778187981918:
3: To Kill a Mockingbird, with distance of 0.6482055113412749:
4: Brave New World, with distance of 0.6536931421330112:
5: The Poisonwood Bible, with distance of 0.6585409808008259:

```