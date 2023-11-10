# Bias-and-Fairness-Assessment-of-Models

### The goal of this project is to explore the concept of bias through querying an existing natural language processing model — specifically, the Perspective API released by Google Jigsaw. In this project, I examine a dataset of internet comments and their scores, in addition to formulating my own queries and using the Perspective API client to score the toxicity of each comment.

### Hypothesis: The Perspective API will make more mistakes on shorter or more informal pieces of content (like tweets and social media comments) compared to longer ones (like book and movie and reviews) To test my hypothesis, I have gathered 16 short comments and 16 long comments from various social media platforms, customer reviews and blog posts, and tested them with the Perspective API client to check whether it correctly classifies them as toxic or non toxic.

### The data_bias.csv file contains the test data and the data_bias_query.ipynb contains all the code used for my testing and analysis.

### Insights: Based on my results, the accuracy of the model drops by 12.5% for short toxic comments compared to longer ones, suggesting a potential bias in its performance. This difference implies that the model may be predisposed to struggle with shorter, more informal content commonly found in social media comments and tweets.

### The informal nature of shorter comments, especially in the form of slang and expressions found in social media comments and tweets, may introduce bias by making it more challenging for the Perspective API to accurately interpret and classify toxicity. Longer comments like book and movie reviews offer a more comprehensive language context, which potentially reduces any bias in the API model's evaluation.

### These findings suggest that users should be mindful of the model's potential limitations and biases in scenarios where content length and informality are involved.
