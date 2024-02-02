# Dataset Description: OnePlus Nord 5G Reviews 

The **OnePlus Nord 5G Reviews Dataset** is a collection of customer reviews sourced from Amazon's platform through the utilization of the BeautifulSoup web scraping tool. This dataset serves as a valuable resource for gaining insights into user sentiments and experiences regarding the smartphone.

Structured in a tabular format, the dataset encompasses the following five key columns:

- **Product Name:** Identifier of the product (OnePlus Nord 5G)
- **Profile Name:** Identifier of the reviewer's profile.
- **Review Title:** Concise title assigned by the reviewer, encapsulating their viewpoint.
- **Review Rating:** Numerical rating granted by the reviewer, indicative of their overall satisfaction level.
- **Review Text:** Comprehensive textual review wherein users elaborate on their experiences, features they appreciated or found lacking, and encountered issues.

The dataset consists of 9,470 individual rows, each representing a distinct review of the smartphone. It is presented in a structured tabular form to facilitate seamless integration and analysis.

- The **Review Rating** column facilitates quantitative evaluation of user satisfaction, enabling computation of sentiment analysis by classification of reviews according to their ratings.
- The detailed **Review Text** column provides rich insights into users' sentiments, preferences, and potential areas for enhancement.

# Pre-processing

**Preprocessing Steps:**

1. **Fixing Contractions:**
   Contractions, such as "can't" and "won't," were expanded into their full forms ("cannot," "will not") to ensure consistent tokenization and analysis.

2. **Removing Punctuations:**
   Punctuation marks were removed from the text, eliminating noise and simplifying the data for subsequent steps.

3. **Removing Numbers:**
   All numerical digits were removed from the text.

4. **Converting to Lowercase:**
   All text was converted to lowercase to standardize the data and prevent duplication of words due to capitalization variations.

5. **Spell Check using TextBlob:**
   The TextBlob library was employed for spell checking, rectifying any obvious spelling errors in the text. This enhances the accuracy of subsequent processing steps.

6. **Tokenization:**
   The text was tokenized, breaking it down into individual words. This is a fundamental step for further analysis as it creates the basic units for subsequent processing.

7. **Lemmatization:**
   Lemmatization was performed to reduce inflected words to their base or root form (e.g., "running" to "run"). This aids in grouping similar words and reducing the dimensionality of the data.

8. **Removing Stop Words:**
   Common stop words (e.g., "the," "and" "is") were removed from the text.

9. **Text Vectorization:**
   Text vectorization was applied to convert the pre-processed text into a numerical format suitable for machine learning. Techniques like TF-IDF (Term Frequency-Inverse Document Frequency) or Count Vectorization were used to represent words as numerical features.

10. **Joining Together:**
    After applying the above steps, the pre-processed tokens were rejoined to form coherent and cleaned review text.

**Benefits of Preprocessing:**
- **Noise Reduction:** Removing punctuations, numbers, and correcting spellings contributes to a cleaner and more focused dataset.
- **Standardization:** Converting all text to lowercase and lemmatization ensure standardized representation of words, reducing variations due to capitalization and inflections.
- **Efficient Analysis:** Removing stop words and irrelevant characters streamlines the data, making it more manageable and efficient for analysis.
- **Enhanced Accuracy:** Spell checking and lemmatization improve the accuracy of subsequent analyses by minimizing errors and focusing on core content.
