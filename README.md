# Conversational-AI

Exercise 1
Tokenization is the first step in text processing. It's the process of breaking text into parts or
tokens. You will use the Natural Language Toolkit (NLTK), a powerful Python library for working
with text.
1.	Install NLTK:
If NLTK is not already installed, we use !pip install nltk to install it.  This step is only required once.
2.	Import Necessary Functions:
We import word_tokenize from nltk.tokenize to break the text into    individual words (tokens).
We import FreqDist from nltk.probability to analyze the frequency of each token.
3.	Define Text:
We define a sample text variable with at least four sentences on the   topic of Natural Language Processing (NLP).
4.	Tokenize Text:
We use the word_tokenize function to split the text into tokens (words and punctuation marks), which are stored in the list tokens.
5.	Display List of Tokens:
The script prints the list of tokens generated from the text variable.
6.	Count Number of Tokens:
Using len(tokens), we calculate and print the total number of tokens    in the text.
7.	Calculate Token Frequency:
          Using FreqDist(tokens), we calculate the frequency of each token.
The frequencies are printed in a readable format showing each token
         With its count.









Exercise 2
It explains how to create a word cloud from a text file stored in Google Drive, visualize it in Google Colab, and upload the completed code to GitHub. Word clouds are a popular text visualization tool, showing word frequencies where larger words represent higher occurrences. Here, we’ll cover the installation, configuration and customization.

1.	Install the WordCloud Library
To generate a word cloud, you’ll first need to install the wordcloud library, which provides tools to create and customize word clouds. This library needs to be installed in the Colab environment if it’s not already available.
2.	Import Required Libraries
After installation, import the necessary libraries:
o	WordCloud and STOPWORDS from the wordcloud library:
	WordCloud allows for generating word clouds.
	STOPWORDS provides a predefined list of common words (e.g., “the,” “and”) to exclude from the word cloud.
o	matplotlib.pyplot to display the word cloud as an image.
3.	Mount Google Drive
Mount your Google Drive in the Colab environment to access files stored in Drive. This allows you to read the text file that you’ll use for generating the word cloud. When you mount Drive, you’ll be prompted to sign in and grant Colab permission to access your files.
4.	Load the Text File
Once Drive is mounted, you can read the text file and load its content. This file should be a .txt file containing the text you want to visualize. Load the file using Python’s open function and store its contents in a variable. The text in this variable will be the input for the word cloud.
5.	Create a WordCloud Object
Configure the WordCloud object with various settings:
o	Size: Set width and height to control the size of the output image.
o	Background Color: Choose a background_color, such as "white" or "black," to change the background.
o	Stopwords: Use STOPWORDS to remove common words from the visualization.
o	Font Size: min_font_size sets the smallest font size for words displayed in the word cloud.
These parameters allow you to customize the appearance of the word cloud to match your visualization needs.
6.	Display the Word Cloud
Use matplotlib.pyplot to display the generated word cloud as an image. This involves setting the display size and rendering the image without additional padding or axes (i.e., x and y-axes are hidden to keep the image clean). Once configured, Colab will display the word cloud as an image in the output cell.

Additional Customization Options

1.	Experiment with Colors and Fonts
Adjust the background_color, min_font_size, and other font settings to change the color scheme and improve readability. Try different colors for the background, or change the color map (color gradient) for words. This can make certain words stand out or suit the theme of your visualization better.
2.	Limit the Number of Words
Use the max_words parameter to control the maximum number of words displayed in the word cloud. This option can help focus on the most frequent words and create a simpler image by filtering out less common words.
3.	View Word Frequencies Separately
If you want to see the word frequencies separately, you can use frequency distribution functions to display the frequency count for each word. This can give insights into the most common terms before visualizing them.
4.	Use a Mask for Custom Shapes
For more advanced customization, use an image as a “mask” to shape the word cloud. For example, a cloud_shape mask will produce a word cloud with that outline. To do this, load a grayscale image of the shape you want (e.g., a .png file with a transparent or white background) and use it as the mask for the WordCloud object.






