Project 2: WordSense Disambiguation in Medical Context
This project aims to contribute to Word Sense Disambiguation in the domains of biomedical and clinical text.


1. Initially study again Lesk implementation in NLTK. Consider the sentence “I have been prescribed two important drugs today during my visit to clinic” and assume that the target word is “drug”. Construct a simple script that outputs the correct sense of “drug” in the above sentence using standard Lesk algorithm. And, comment on the outcome the efficiency of the result.

2. Download and study MSH-WSD dataset from https://github.com/clips/yarn. The database contains 203 ambiguous terms that include regular terms, acronyms. Make a random selection of 10 acronyms and 10 regular terms. Use Lesk algorithm to perform the wordsense disambiguation of each of these 10 acronym and 10 regular terms and use the ground truth to compute the average accuracy on regular terms and average accuracy on acronyms.

3. Study the various disambiguation algorithms implemented in https://github.com/alvations/pywsd. Show that you can run the program on a simple sentence containing a target word to disambiguate and output for various disambiguation algorithms (Original Lesk, adapted/extended Lesk, simple Lesk extended with hypernym and hyponyms, cosine Lesk, path-semantic similarity, Information content-semantic similarity, highest Lemma count.)

4. Run the above various algorithms in 3) on MSH-WSD dataset and report the average accuracy on all acronyms and average accuracy on all regular terms.

5. We would like to extend similarity-based Lesk algorithm to include phonetic matching, which evaluates phonetically similar wording. For this purpose, use the “Fuzzy” library in python to generate the character string that identifies phonetically similar words, and then use edit distance to compute the phonetic similarity between two words. See an example of implementation at https://www.analyticsvidhya.com/blog/2017/01/ultimate-guide-to-understand-implement-natural-language-processing-codes-in-python/.  Demonstrate this reasoning on the example sentence pointed out in 1) and generate a matrix that indicates the phonetic distance between each pair of words of the sentence.

6. We would like to extend the Wu and Palmer-semantic similarity extension of Lesk algorithm implemented in 3) by incorporating the phonetic similarity as well so that the overall similarity is computed as a convex combination of Wu and Palmer similarity and phonetic similarity (after being normalized) with coefficient of 0.5. Suggest and an implementation and run your new code on selected MSH-WSD dataset.

7. Suggest a GUI of your choice that allows the user to visualize the various outputs of the disambiguation task. Ideally the use can input a sentence and a target word to be disambiguated.

8. Comment on the overall finding.
