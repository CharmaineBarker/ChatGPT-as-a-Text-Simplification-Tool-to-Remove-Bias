# ChatGPT-A Text Simplification Tool as an Application for Removing Bias
The work for a paper submitted to Yorkshire Innovation in Science and Engineering Conference 2023 generated a dataset of Disneyland reviews which is released here.

The sample of 300 reviews was taken from a Kaggle dataset: [Disneyland Reviews](https://www.kaggle.com/datasets/arushchillar/disneyland-reviews)

Each review was then manually inputted into [ChatGPT](https://chat.openai.com/) using the prompt: Simplify "(Review)". The output was then added to a new column in the dataset. The dataset contains the following features:

* `Reviewer_Location`- The sensitive attribute which was country of origin of the reviewer. This was filtered to only have 150 people from the `United Kingdom` and 150 from the `United States`.
* `American`- This is the same as the `Reviewer_Location` column, but it has been changed into a binary where `1` is United states and `0` is United Kingdom.
* `Review_Text`- The actual review data which was simplified.
* `Prompt`- This is the text which was used as the input into ChatGPT.
* `Simplified`- This is the output from ChatGPT.

A number of tests were completed on this data such as sentiment analysis to check the reviews kept the same meaning and classification of thje reviews into one of the two protected characteristics (UK or US). Further Work is also outlined in the paper.
