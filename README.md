# Movie Recommendation System by Mahesh

A high performance recommendation engine that uses content based filtering to suggest movies based on user preferences. This project uses data processing, vectorization, and SQL database management.

## Tech Stack Used :
 Python: Core logic.
 Scikit-Learn: For the recommendation engine (CountVectorizer and Cosine Similarity).
 Pandas & NumPy: For data manipulation and matrix operations.
 SQLite: Used for storing movie metadata and user profiles.
 Rich: For a polished terminal interface.

##  Database Architecture :
The system relies on a structured SQLite database (`movies.db` ) with three primary tables:
1. Movies Table: Contains titles, genres, directors, stars, and keywords.
2. Users Table: Manages user profiles and credentials.
3. Users_data Table: Tracks user ratings and liked movies to build a preference profile.

##  How the Engine Works
1. Normalization: Applies Min-Max normalization to movie scores.
2. Feature Extraction: Uses NLP techniques to extract attributes from keywords and genres.
3. Similarity Calculation: Executes the engine process to find the closest matches in the database.

##  Setup
Install the dependencies:
```bash
pip install -r requirements.txt

python src/main.py

## For Quick Start & Login
To explore the recommendation engine, use the following credentials:
User ID: mahesh
Password: 1234

### How to Run
1. Install dependencies: `pip install -r requirements.txt`
2. Run the application: `python src/main.py`

