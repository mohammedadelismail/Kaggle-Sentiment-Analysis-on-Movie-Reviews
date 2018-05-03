# Sentiment Analysis on Movie Reviews

This is solution implementation to Kaggle's [Sentiment Analysis on Movie Reviews](https://www.kaggle.com/c/sentiment-analysis-on-movie-reviews) competition.

This Competition goal is to apply sentiment analysis techniques on [Rotten Tomatoes dataset](https://www.rottentomatoes.com/).

<b>Quoting from Kaggle's:</b><br/>

The dataset is comprised of tab-separated files with phrases from the Rotten Tomatoes dataset. <br/>
The train/test split has been preserved for the purposes of benchmarking, but the sentences have been shuffled from their original order.<br/>
Each Sentence has been parsed into many phrases by the Stanford parser. <br/>
Each phrase has a PhraseId. <br/>
Each sentence has a SentenceId. <br/>
Phrases that are repeated (such as short/common words) are only included once in the data.<br/>


<b>Submission Evaluation</b><br/>
Submissions are evaluated on classification accuracy (the percent of labels that are predicted correctly) for every parsed phrase.<br/>
The sentiment labels are:
- 0 - negative
- 1 - somewhat negative
- 2 - neutral
- 3 - somewhat positive
- 4 - positive

This solution got overall <b>accuracy = 0.63392</b> on the test set.

The model used in this solution is <b>LinearSVC</b> with <b>tf-idf</b> based feature vector.

Some another experiments have been done with different features extraction approaches and ML techniques but the one presented in this notebook is the one with the best results.