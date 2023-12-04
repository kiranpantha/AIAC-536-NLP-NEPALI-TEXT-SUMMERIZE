# AIAC-536-NLP-NEPALI-TEXT-SUMMERIZE
Nepali Text Summarization using TF-IDF (Term Frequency-Inverse Document Frequency)

**Extractive Summarization of Nepali Text using TF-IDF**

**Objective**The goal of this project is to implement an extractive text summarization technique tailored for the Nepali language. The project focuses on leveraging the Term Frequency-Inverse Document Frequency (TF-IDF) method to identify key sentences and generate concise summaries.


## Dataset/Corpus

The project will draw from a meticulously curated Nepali language dataset, incorporating a diverse array of textual content. This dataset will include sources such as news articles, blogs, and literature, covering a broad spectrum of Nepali language usage. The selection process will prioritize data relevance, linguistic diversity, and cultural representation to ensure the model's effectiveness across various domains.


## Project Idea

The primary goal is to craft an advanced extractive text summarization system specifically tailored for the Nepali language. The proposed system will harness the power of the TF-IDF (Term Frequency-Inverse Document Frequency) method, employing a multifaceted approach to process Nepali sentences. The workflow involves sophisticated steps, including tokenization, the creation of word frequency matrices, calculation of TF-IDF scores, and the generation of succinct summaries. The project's broader vision is to fill the gap for an efficient text summarization tool catering to the linguistic intricacies and cultural nuances unique to Nepali. The resulting system aims to empower users, enabling them to swiftly distill essential information from Nepali texts and enhancing overall content comprehension.


## Software and Tools to be Used

The Natural Language Toolkit (NLTK) will be a central component, serving as the primary library for language processing tasks. Complementary tools such as Pandas and NumPy will be strategically employed for seamless data preprocessing and insightful analysis. 

The development environment will be structured around Jupyter Notebooks, offering an interactive and iterative platform for code execution and comprehensive documentation. The chosen suite of tools reflects a meticulous consideration of efficiency, versatility, and maintainability throughout the project's lifecycle.


## Teammates and Work Division

As the sole contributor to this project, the responsibility for both linguistic and technical aspects rests with the project initiator. The individual will play a dual role, overseeing linguistic facets to ensure precision in language processing and providing valuable insights into the cultural intricacies inherent to Nepali. Simultaneously, the project initiator will drive the technical implementation, encompassing tasks such as code development, dataset preprocessing, and the seamless integration of the TF-IDF algorithm. The work plan is structured to foster a holistic and integrated approach to the development of the Nepali text summarization system.

This solo project demands a disciplined and self-driven work ethic, underpinned by a systematic approach to project management. Regular self-assessment and progress tracking mechanisms will be in place to ensure milestones are met efficiently. The project initiator will maintain a flexible and adaptive mindset, accommodating any challenges that may arise during the development process. The overarching objective is to create a robust and effective solution that aligns with the unique linguistic and cultural context of the Nepali language.


### Source Code

The project's source code is written in Python, making use of the Natural Language Toolkit (NLTK) library. It comprises functions responsible for creating word frequency matrices, calculating TF-IDF scores, and generating Nepali language summaries.


Code Structure\
Function Descriptions
---------------------

**create\_word\_frequency\_matrix(sentences)**

Purpose: Tokenizes Nepali sentences and creates a word frequency matrix for each sentence.

Usage: word\_frequency\_matrix = create\_word\_frequency\_matrix(sentences)

**create\_term\_frequency\_matrix(word\_frequency\_matrix)**

Purpose: Creates a term frequency matrix from the word frequency matrix.

Usage: term\_frequency\_matrix = create\_term\_frequency\_matrix(word\_frequency\_matrix)

**create\_document\_frequency\_table(word\_frequency\_matrix)**

Purpose: Creates a table indicating how many documents (sentences) contain each Nepali word.

Usage: doc\_frequency\_table = create\_document\_frequency\_table(word\_frequency\_matrix)

**create\_inverse\_document\_frequency\_matrix(word\_frequency\_matrix, doc\_frequency\_table, total\_documents)**

Purpose: Creates an inverse document frequency matrix specific to the Nepali language.

Usage: inverse\_document\_frequency\_matrix = create\_inverse\_document\_frequency\_matrix(word\_frequency\_matrix, doc\_frequency\_table, total\_documents)

**create\_term\_frequency\_inverse\_document\_frequency\_matrix(term\_frequency\_matrix, inverse\_document\_frequency\_matrix)**

Purpose: Creates a term frequency-inverse document frequency matrix tailored for Nepali text.

Usage: tf\_idf\_matrix = create\_term\_frequency\_inverse\_document\_frequency\_matrix(term\_frequency\_matrix, inverse\_document\_frequency\_matrix)

**calculate\_sentence\_scores(tf\_idf\_matrix)**

Purpose: Calculates sentence scores for Nepali sentences based on TF-IDF.

Usage: sentence\_scores = calculate\_sentence\_scores(tf\_idf\_matrix)

**calculate\_average\_sentence\_score(sentence\_scores)**

Purpose: Calculates the average score of Nepali sentences.

Usage: average\_score = calculate\_average\_sentence\_score(sentence\_scores)

**generate\_summary(sentences, sentence\_scores, threshold)**

Purpose: Generates a Nepali language summary based on the sentence scores and a specified threshold.

Usage: summary = generate\_summary(sentences, sentence\_scores, threshold)


### Input and Output

Input: The user provides Nepali text for summarization.

Output: The code produces an extractive summary in the Nepali language.


## Usage Example

**# User input for the Nepali text to be summarized**

text = input("निरिक्षण गर्न चाहिएको पाठ लेख्नुहोस्:\n\n")

**# Tokenizing Nepali sentences**

sentences = re.split('।', text)

**# ... (Code to process Nepali text and generate a summary)**

print(summary)

print(f"Length of the summary: {len(summary)}")


## Conclusion

This project showcases the implementation of an extractive text summarization technique tailored for the Nepali language. The code follows a modular approach to process Nepali text and generate concise summaries. The use of the TF-IDF method enables the identification of key sentences based on word frequency and importance in Nepali documents.


## Future Improvements

1. Potential enhancements for future iterations of this project may include:

2. Incorporating sentence importance thresholds for increased customization.

3. Exploring additional natural language processing techniques to improve the accuracy of summarization.

4. Optimizing the code for efficient handling of larger Nepali language datasets.
