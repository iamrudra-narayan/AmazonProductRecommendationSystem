# AmazonProductRecommendationSystem

Find the complete code, dataset and Reference by <b><a href="https://drive.google.com/drive/folders/10KGTcF5VBebyDFEQlmVTpJTsSCX9b4sB?usp=sharing">CLICKING HERE</a></b>

<img src="https://github.com/iamrudra-narayan/AmazonProductRecommendationSystem/assets/84215414/e41b7126-9248-47d8-8b3c-8775078b18f1">
<br>
<h2><b>INTRODUCTION</b></h2>
<br>
In this notebook, we aim to tackle the real-world problem of building a recommendation system for Amazon products. Recommendation systems play a crucial role in e-commerce platforms like Amazon by helping users discover products that they might be interested in based on their preferences and behavior. In this project, we'll explore various techniques and algorithms to develop a recommendation system that provides personalized and relevant product recommendations to Amazon users.
<br>
<br>
<h2><b>ABOUT DATASET</b></h2>
<br>
<b>Find the Complete Dataset by <a href="https://drive.google.com/drive/folders/1WLNHqePrioUnpowv6xpu6l0Cb0VQ27BB?usp=sharing">CLICKING HERE</a></b>
<br>
<h4><b>Download the dataset from kaggle:- </b></h4> <a>https://www.kaggle.com/datasets/lokeshparab/amazon-products-dataset</a>
<br>
**main_category:**

This column represents the main category or department to which the product belongs.
Examples of main categories include electronics, clothing, home decor, books, etc.

***sub_category:***

This column provides additional categorization within the main category.
For example, within the electronics category, sub-categories could include smartphones, laptops, headphones, etc.

***image:***

The image column contains URLs or file paths to images of the products.
These images are typically used for visual representation of the products on the e-commerce platform.

***link:***

The link column contains URLs to the product pages on the e-commerce website.
Users can click on these links to view detailed information about the products and make purchases.

***ratings:***

This column contains the average rating of the product, typically on a scale of 1 to 5.
Ratings are provided by users who have purchased or interacted with the product and are used to measure customer satisfaction.

***no_of_ratings:***

The no_of_ratings column represents the total number of ratings or reviews received by the product.
It indicates the level of engagement and popularity of the product among users.

***discount_price:***

This column contains the discounted price of the product, if applicable.
Discounts are often offered by e-commerce platforms to attract customers and increase sales.

***actual_price:***

The actual_price column contains the original or list price of the product before any discounts.
It provides users with information about the product's original value and helps them assess the savings offered by discounts.
<br>
<br>
<h2><b>Approaches for Feature Engineering</b></h2>
<br>
**image_vec:**

Use techniques such as image embedding or convolutional neural networks (CNNs) to extract features from product images.
Apply pre-trained image models such as **EfficientNetB1** to extract high-level features from images.
Use dimensionality reduction techniques (e.g., PCA) to reduce the dimensionality of image features while retaining important information.
Normalize image features to ensure consistency and improve model performance.

***name_vec:***

Use techniques such as word embedding such as **Sent2Vec** to convert product names into dense vector representations.

***name_bow:***

Convert product names into a Bag-of-Words (BoW) representation, where each word in the name is represented as a feature with its frequency count.
Use TF-IDF (Term Frequency-Inverse Document Frequency) to weigh the importance of words in product names based on their frequency in the dataset.
Here the dimension is 5000, because the 4729 dimensions covers 94% of the variance Information.

***discounted_percentage:***

Calculate the discounted percentage by subtracting the discounted price from the actual price and dividing by the actual price.
Normalize the discounted percentage to ensure consistency and scale it to a standard range (e.g., between 0 and 1).

***discounted_price_norm:***

Normalize the discounted price to ensure consistency and scale it to a standard range (e.g., between 0 and 1).
Use techniques such as min-max scaling or z-score normalization to scale the discounted prices based on the distribution of values in the dataset.

***ratings_norm:***

Normalize the ratings to ensure consistency and scale them to a standard range (e.g., between 0 and 1).
Use techniques such as min-max scaling or z-score normalization to scale the ratings based on the distribution of values in the dataset.

***image_vec_norm:***

Normalize the image features extracted using techniques like min-max scaling or z-score normalization.
Ensure that image features are scaled to a standard range to improve model performance and consistency.
<br>
<br>
<h2><b>CONCLUSION</b></h2>
<br>
<ul>
  <li>
    In conclusion, this notebook provides a comprehensive overview of building a recommendation system for Amazon products, from data preprocessing and exploratory analysis to model implementation and deployment. By leveraging the techniques and methodologies discussed in this project, e-commerce platforms like Amazon can improve customer satisfaction, drive sales, and stay competitive in the ever-evolving online marketplace.
  </li>
</ul>
<br>
<br>
<h2><b>REFERENCES</b></h2>
<br>
<ol>
    <li><b>Kaggle:</b> https://www.kaggle.com/datasets/lokeshparab/amazon-products-dataset</li>
    <li><b>Keras-EfficientNetB0-B7: </b> https://keras.io/api/applications/efficientnet/</li>
    <li><b>Sent2Vec: </b> https://pypi.org/project/sent2vec//</li>
</ol>
<br>
<br>
<h1><b>THANK YOU</b></h1>
