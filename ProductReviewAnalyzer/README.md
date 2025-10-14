These code blocks are configuration entries for a Java project that utilize Stanford CoreNLP, a suite of natural language processing tools developed by Stanford University.

Purpose of Stanford CoreNLP

Stanford CoreNLP provides a collection of language analysis tools that enable computers to process and understand human language. One of its key features is sentiment analysis, which determines the emotional tone (such as positive, negative, or neutral) of a piece of text.

This dependency adds the language models required by CoreNLP. These models are essential datasets that enable the library to analyze and interpret human language accurately.

Why Are There Two Dependencies?
    The first dependency brings in the program logic—the actual algorithms and methods for processing text.
    The second dependency provides the data models needed for these algorithms to function, such as language rules and sentiment patterns.

This application uses StanfordNLP model that is pre-trained for sentiment analysis and can categorize the sentiments into 5 categories.
- Very Positive
- Positive
- Neutral
- Negative
- Very Negative

The main class of this application is ProductReviewAnalyzer. Click the button below to open and observe the content of the file.

Explanation of the ProductReviewAnalyzer class

The program analyzes the sentiment of product reviews using Stanford CoreNLP, a natural language processing library.

It reads reviews from a CSV file with the help of the OpenCSV library.

The code first sets up a pipeline that can break text into sentences and determine the overall feeling (sentiment) of each sentence.

For each review, it finds the sentiment of the longest sentence and uses that as the main sentiment for the whole review.

Sentiments are classified into five categories: Very Positive, Positive, Neutral, Negative, and Very Negative.

As it processes each review, it keeps track of how many reviews fall into each sentiment category.

After all reviews are analyzed, it prints out a report showing the number and percentage of reviews in each sentiment type, along with a simple visual bar to make the results easier to see.

The program includes error handling to deal with issues like missing files or problems reading the CSV data.

In summary, this code shows how to use Java to automatically check if customer feedback is positive or negative and summarize the results in an easy-to-read format.

This application is a Product Review Sentiment Analyzer that is created using Stanford CoreNLP for natural language processing and OpenCSV to read review data from a CSV file.

Running the Application
When you run this application,
    -it initializes the analyzer and NLP pipeline.
    -loads reviews from a CSV file using OpenCSV.
    -returns a list of string arrays (String[]) where each array is a row from   the CSV.
    -For each review,
        Analyzes the sentiment.
        Prints a shortened version of the review with its sentiment.
    -Finally, calls generateReport() to summarize sentiment stats.