# text-augmented-Flickr47
Flickr47 is a public logo dataset that contains 27 logos and 20 text-only logos, which has served as a popular benchmark for evaluating logo detection algorithms. Each image in the dataset is annotated with one or more pairs of bounding box and class label for the logo. Each class has 30 and 10 annotated images for training and testing respectively. Among the 10 testing images for each class, 5 of them have the brand logos while the other 5 only have background image without any logos. 

To generate relevant textual information for the brands, we retrieved content from the brands' wikipedia page whereas for the no-logo background class images, we used the wikipedia content for term "Wikipedia". We enforce each selected sentence to have at least 5 words. For each picture, we randomly select one sentence among all the relevant sentences in its corresponding class. Due to the fact that the number of available sentences for each class varies from class to class, different pictures from the same class might be assigned with the same sentence.

The text files are named after the a similar naming convention of the original flickr47 ground truth files. For instance, if the original flickr47 file name is 000000000.gt_data.txt, the new file containing the augmented text will be named as 000000000.gt_data_text.txt within which the added last column contains the text.
