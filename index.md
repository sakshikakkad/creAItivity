# Art Mood Identifier
**by team creAItivity - Sakshi, Anna, Ahn, TK, Nathan**

### Introduction
In recent years, developments in digital media technologies as well as easy access to content (through social media platforms and other online sources) require developments in data retrieval and processing tools. Images can be categorized by metadata (keywords or tags) or can be retrieved through content-based image retrieval systems, which classify images based on information contained within the images themselves. However, it is still difficult to retrieve and classify images based on variable, “human” characteristics such as emotion.  

### Problem
We propose to train a machine learning model to classify images based on their associated emotions. The ability to classify images in this way would be useful for social media platforms and image retrieval tools, as it would allow access to more relevant digital media through queries made with “human” parameters rather than empirical ones. Social media platforms and marketing agencies can more accurately display and recommend content for users when algorithms are better trained to interpret data qualitatively.  

### Approach
Our dataset will come from online databases such as Flickr and Wikimedia commons. We will classify these images in our machine learning model based on the Reisenzein mood model, which organizes emotions in 2 dimensions based on valence and arousal. We will gather 2000 images per category, resulting in a total of 8000 images. 

![Image](https://github.com/Nathan-Wang-GT/crealtivity.github-io/blob/gh-pages/ModelWithImages.jpg)

We plan on using a Deep Learning algorithm (Convolutional Neural Network) to analyze our data. We will either use public CNN architectures such as ResNet or VGG-16, or create our own using python. We will analyze the HSV color content of the images (hue, saturation, value), as well as other potential features including shapes and textures. We will then map these images based on their features to the four different emotion sets. 

![Image](https://github.com/Nathan-Wang-GT/crealtivity.github-io/blob/gh-pages/HSV.png)

We will first run this model based on our original dataset of 8000 images, then again on a modified dataset of rotated/inverted images to see if the model Is improved. Another parameter to consider is the inclusion of people in images, as facial features or other characteristics of people can influence the “mood” of an image.  

### Potential Results
We expect that the inclusion of people in images could skew the results because the model may not pick up on these characteristics. We also expect to see the model categorize images with warmer hues, higher saturation, and a higher value (more bright) as euphoric (quadrant 1 on the Reisenzein model), while images with cooler hues, lower saturation, and lower values will be classified as melancholy (quadrant 3). 

![Image](https://github.com/Nathan-Wang-GT/crealtivity.github-io/blob/gh-pages/PotentialResults.jpg)

### Timeline
![Image](https://github.com/Nathan-Wang-GT/crealtivity.github-io/blob/gh-pages/timeline%20updated.png)

### References
1. [Content-based mood classification for photos and music: a generic multi-modal classification framework and evaluation approach](https://dl.acm.org/doi/abs/10.1145/1460096.1460114)
2. [Building Emotional Machines: Recognizing Emotions through Deep Neural Networks](https://arxiv.org/abs/1705.07543)
3. [Image Retrieval by Emotional Semantics: A Study of Emotional Space and Feature Extraction](https://ieeexplore.ieee.org/document/4274431)
