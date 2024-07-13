# CONTENT BASED FILTERING

# Product Recommendation using OpenAI Embeddings 
![screenshot](rec.png)
This repository contains the code and documentation for a Product Recommender System built using machine learning techniques.

## Introduction
The Product Recommender System is designed to suggest products to users based on their preferences and past behaviors. 
This system utilizes various openai text embedding and cosine similarity to provide accurate and personalized recommendations for a user whoes history of liked items is known.
The recommendation is evaluated using PCA.

## Dataset
The products data consist of product information such as product_Id, title and description.

## Data Processing
The raw data is processed to add a new colum product_status which siggest if the product is viewed by a user we have considerd for this usecase
The title and discription columns are combined before converting it to text embeddings
An openAI embedding model is used to converet combined product information into vectors 

## Modling
A vector based cosine similarity search is used to find the top similar products that aligns with the user view history

## Evaluation
The model output of top n suggestions or recommendation is viewed as a 2D vector using PCA which shows how close the recommendation is w.r.t the user view history. Visualizations are included to provide insights into the effectiveness of the recommender system.

## Contributing
Contributions are welcome! Please read the contributing guidelines first.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
