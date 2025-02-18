# AI/Machine Learning Intern Challenge: Simple Content-Based Recommendation

**By: Mythri Kishore**

---

## Dataset
The dataset used for this AI/ML challenge is sourced from [Kaggle](Kaggle.com).

Specifically, I used the [IMDB Top 250 Movies Dataset](https://www.kaggle.com/datasets/rajugc/imdb-top-250-movies-dataset). To access the data, click the link and select the download button to download the csv file as a zip file. Place it into an appropriate location on your device. Then, use the corresponding file path to load the data into the Jupyter Notebook. Directions are also included in the notebook itself.

The downloaded csv file is also included in the repository: `IMDB_Top_250_Movies.csv`

## Setup
The code is meant to be run in a Jupyter Notebook with Python 3. The necessary imports are included in the first code cell of the notebook. If you receive a message saying `Requirement already satisfied....` it is safe to continue with the execution of subsequent cells.


## Running
To run the recommender function and process the text data, open the Jupyter Notebook from the repository: `recommendation_system.ipynb`. 

## Results
**Example input:**
`recommend_movies("A thrilling space adventure with humor")`

**Example output:**
`[('Alien', 0.343),
 ('How to Train Your Dragon', 0.245),
 ('2001: A Space Odyssey', 0.23),
 ('Children of Heaven', 0.225),
 ('Lawrence of Arabia', 0.224)]`

The output is formatted as a list containing 5 tuples which are the closest movie matches to the input string based on TF-IDF cosine similarity. Tuples are in the form: `(Movie_name, similarity_score)`. Similarity scores can take a value in the range 0 to 1.

