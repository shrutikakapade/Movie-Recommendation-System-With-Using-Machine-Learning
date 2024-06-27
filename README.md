<h1 align="center">Project Description: Movie Recommendation System Using Machine Learning</h1>
<hr>
<h2>Overview :</h2>
<p align="left">This project aims to build a movie recommendation system using machine learning techniques. The system leverages various Python packages such as numpy, pandas, ast, sklearn, and nltk for data processing, feature extraction, and natural language processing. Additionally, streamlit is used for developing a user-friendly web application to interact with the recommendation system.</p>
<h2>Data Description:</h2>
<h3>We use two primary datasets:</h3>
<p>
- Movies Data: This dataset contains information about movies, including attributes such as       budget, genres, homepage, id, keywords, original language, original title, overview,            popularity, production companies, production countries, release date, revenue, runtime,         spoken languages, status, tagline, title, vote average, and vote count.
  
- Credits Data: This dataset includes information about the cast and crew of the movies, with     attributes such as movie_id, title, cast, and crew.</p>
<h2>Data Preprocessing:</h2>
<p>
- Merging Datasets:
  Merge the movies and credits datasets on the common attribute, typically movie_id or id.
  Cleaning and Transforming Data:

- Handle missing values and inconsistencies.
  Extract relevant information from nested columns such as genres, keywords, cast, and crew       using the ast library.
  
- Natural Language Processing:
  Use the nltk library, particularly the 'PorterStemmer' class, to stem text data. This involves   reducing words to their base or root form to ensure consistency in text-based features.
</p>
<h2>Feature Engineering:</h2>
<p>
- Text Vectorization:
  Convert textual data such as genres, keywords, overview, cast, and crew into numerical          vectors using techniques like TF-IDF (Term Frequency-Inverse Document Frequency) from           sklearn.feature_extraction.
  
- Distance Calculation:
  Compute the cosine similarity between movie vectors. Cosine similarity is preferred over        Euclidean distance due to its effectiveness in high-dimensional spaces and its ability to       measure the cosine of the angle between vectors, indicating their orientation and,              consequently, their similarity.</p>
<h2>Machine Learning Model</h2>
<p>
- Similarity Calculation:
  For each movie, calculate its similarity with every other movie using cosine similarity.
  Recommend movies based on the highest similarity scores.</p>

<h2>Web Application: </h2>
<p>
- Building the App:
  <ul>
    <li>Use streamlit to develop an interactive web application.</li>
    <li>Load the preprocessed data and model using pickle.</li>
    <li>Create a user interface to input a movie title and fetch recommendations.</li>
</ul>
- API Integration:
 <ul>
<li>Use the requests library to fetch additional data from external APIs if needed (e.g., movie posters, additional details).</li></ul></p>
<h2>Conclusion:</h2>
<p>This movie recommendation system effectively utilizes machine learning techniques and natural language processing to provide personalized movie suggestions. By integrating various Python libraries for data processing, feature extraction, and web application development, we deliver a robust and interactive user experience.</p>



