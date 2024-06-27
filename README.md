<h1 align="center">Project Description: Movie Recommendation System Using Machine Learning</h1>
<h3>Overview :</h3>
<p align="left">This project aims to build a movie recommendation system using machine learning techniques. The system leverages various Python packages such as numpy, pandas, ast, sklearn, and nltk for data processing, feature extraction, and natural language processing. Additionally, streamlit is used for developing a user-friendly web application to interact with the recommendation system.</p>
<h3>Data Description:</h3>
<h4>We use two primary datasets:</h4>
<p><ul> 
<li>
Movies Data: This dataset contains information about movies, including attributes such as budget, genres, homepage, id, keywords, original language, original title, overview,popularity, production companies, production countries, release date, revenue, runtime, spoken languages, status, tagline, title, vote average, and vote count.</li>
<li>Credits Data: This dataset includes information about the cast and crew of the movies, with attributes such as movie_id, title, cast, and crew.
</li></ul></p>

<h3>Data Preprocessing:</h3>

<p>
<ul><li>Merging Datasets:</li></ul>
  - Merge the movies and credits datasets on the common attribute, typically movie_id or id.
<ul><li>Cleaning and Transforming Data:</li></ul>
- Handle missing values and inconsistencies.</li></ul>
- Extract relevant information from nested columns such as genres, keywords, cast, and crew using the ast library.</li></ul>
<ul><li>Natural Language Processing:</li></ul>
- Use the nltk library, particularly the 'PorterStemmer' class, to stem text data.This   involves reducing words to their base or root form to ensure consistency 
  in text-based features.
</p>

<h3>Feature Engineering:</h3>
<p align="left">
<ul><li>Text Vectorization:</li></ul>
  Convert textual data such as genres, keywords, overview, cast, and crew into numerical vectors using techniques like TF-IDF (Term Frequency-Inverse 
  Document Frequency) from sklearn.feature_extraction.
  
<ul><li> Distance Calculation:</li></ul>
  Compute the cosine similarity between movie vectors. Cosine similarity is preferred over Euclidean distance due to its effectiveness in high-dimensional spaces 
  and its ability to measure the cosine of the angle between vectors, indicating their orientation and, consequently, their similarity.</p>
  
<h3>Machine Learning Model</h3>
<p align="left">
<ul><li>Similarity Calculation:
  For each movie, calculate its similarity with every other movie using cosine similarity.
  Recommend movies based on the highest similarity scores.</p>

<h3>Web Application: </h3>
<p align="left">
<ul><li>Building the App:</li></ul>
  -Use streamlit to develop an interactive web application.
  - Load the preprocessed data and model using pickle.
  - Create a user interface to input a movie title and fetch recommendations.
<ul><li>API Integration:</li></ul>
  - Use the requests library to fetch additional data from external APIs if needed (e.g., movie posters, additional details).</li></ul></p>
<h3>Conclusion:</h3>
<p align="left">This movie recommendation system effectively utilizes machine learning techniques and natural language processing to provide personalized movie suggestions. By integrating various Python libraries for data processing, feature extraction, and web application development, we deliver a robust and interactive user experience.</p>



