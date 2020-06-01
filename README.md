# MNIST Digit Recognition
A Logistic Regression machine learning model that do takes the mnist_784 data from sklearn and predicts the digits from images.

## The Flow
- Fetch dataset from openml by name or dataset id
- We take mnist_784
- Specify the features and labels ie the data and target
- Take some of the features from the data ==> features *
- Reshape this into 28 x 28
- Show it over pyplot
- Split the data into training and testing
- Randomly shuffled or permute the taken data points
- Split the shuffled data into training and testing
- For the Logistic Regression Classifier, give the tolerance of 0.1. Which is the stoping criteria
- Predict over the taken some of the features from whole *
- Find the cross validation socre
- Whose mean is, in our case, 0.9783666666666667

## The Data
- **Author**: Yann LeCun, Corinna Cortes, Christopher J.C. Burges  
- **Source**: [MNIST Website](http://yann.lecun.com/exdb/mnist/) - Date unknown  
- **Please cite**: The MNIST database of handwritten digits with 784 features, raw data available at: http://yann.lecun.com/exdb/mnist/.    It can be split in a training set of the first 60,000 examples, and a test set of 10,000 examples  \n\nIt is a subset of a larger set available from NIST. The digits have been size-normalized and centered in a fixed-size image. It is a good database for people who want to try learning techniques and pattern recognition methods on real-world data while spending minimal efforts on preprocessing and formatting. The original black and white (bilevel) images from NIST were size normalized to fit in a 20x20 pixel box while preserving their aspect ratio. The resulting images contain grey levels as a result of the anti-aliasing technique used by the normalization algorithm. the images were centered in a 28x28 image by computing the center of mass of the pixels, and translating the image so as to position this point at the center of the 28x28 field.  
  With some classification methods (particularly template-based methods, such as SVM and K-nearest neighbors), the error rate improves when the digits are centered by bounding box rather than center of mass. If you do this kind of pre-processing, you should report it in your publications. The MNIST database was constructed from NIST's NIST originally designated SD-3 as their training set and SD-1 as their test set. However, SD-3 is much cleaner and easier to recognize than SD-1. The reason for this can be found on the fact that SD-3 was collected among Census Bureau employees, while SD-1 was collected among high-school students. Drawing sensible conclusions from learning experiments requires that the result be independent of the choice of training set and test among the complete set of samples. Therefore it was necessary to build a new database by mixing NIST's datasets. 
  The MNIST training set is composed of 30,000 patterns from SD-3 and 30,000 patterns from SD-1. Our test set was composed of 5,000 patterns from SD-3 and 5,000 patterns from SD-1. The 60,000 pattern training set contained examples from approximately 250 writers. We made sure that the sets of writers of the training set and test set were disjoint. SD-1 contains 58,527 digit images written by 500 different writers. In contrast to SD-3, where blocks of data from each writer appeared in sequence, the data in SD-1 is scrambled. Writer identities for SD-1 is available and we used this information to unscramble the writers. We then split SD-1 in two: characters written by the first 250 writers went into our new training set. The remaining 250 writers were placed in our test set. Thus we had two sets with nearly 30,000 examples each. The new training set was completed with enough examples from SD-3, starting at pattern # 0, to make a full set of 60,000 training patterns. Similarly, the new test set was completed with SD-3 examples starting at pattern # 35,000 to make a full set with 60,000 test patterns. Only a subset of 10,000 test images (5,000 from SD-1 and 5,000 from SD-3) is available on this site. The full 60,000 sample training set is available. 
  Downloaded from openml.org.
