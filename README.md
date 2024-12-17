# spot-AI-images
Python code for recognizing AI jpg images through pixel patterns

## Required Libraries
1. `PIL`: Python Imaging library, possibly already built into Python, if not: `pip install pillow` in the command line (Windows) or `brew install pillow` (Mac)
2. `numpy`: Numerical Python, can install by: `pip install numpy` (Windows) or `brew install numpy` (Mac)

## Notes on Analyzing the Data
Usually, AI images have a much lower standard deviation and average than a real image. Real images tend to have larger standard deviations than their AI counterparts, and extremely high averages ranging all the way into the 10,000 range in some cases. This is also extremely dependent on the size of the image. The smaller the image, the harder it is to tell if it's AI.

### For the most accurate results
To further increase accuracy, find an image similar to the suspected AI image you are assessing. If your similar image (which you need to know if it is AI or real, either work) has a significantly higher standard deviation/average, it is most likely real. If it has a significantly lower standard deviation/average, it is most likely AI. (For example, if you have two similar pictures, one with a standard deviation/average of 400/300, and the other with 700/500, the first picture would be most likely AI generated)

## Sample Images
The following websites have both AI and Real images that can be saved and processed through this code:

[Scottsdale Community College Quiz](https://library.scottsdalecc.edu/RealAI)

[Britannica Education](https://elearn.eb.com/real-vs-ai-images/)

[CNet](https://www.cnet.com/pictures/ai-or-not-ai-can-you-spot-the-real-photos/)
