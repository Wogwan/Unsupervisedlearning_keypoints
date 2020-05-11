## 1 Blackground

This program was the learning assignment in the lecture MAEG5735 Applied Intelligence in the CUHK MAE MSc project, which was hosted by [Prof. Wang Changlin](http://www.mae.cuhk.edu.hk/~cwang/) and TA Mr. Liu Zishun. During this lecture, we have learned the basic concept of the Machine Learning and used the Deep Learning methods doing the feature engineering including: labeling, classification in Colab. Here are the 4 demos of the corresponding outputs of the 4 assignments in this lecture:

### 1.1 Assignment 1

In assignment 1, we have defined the import concepts of the body key-points, which could help the tailors to design suitable clothes personally. And the key-points as shown in figure 1.1.

![图片](https://uploader.shimo.im/f/8XPEWf91ApIlnpHe.png!thumbnail)

Figure 1.1 Keypoints illustrations and the generated raw features

As we see, the keypoints are concluded in table1.1:

Table 1.1 Keypoints illustrations

| Side view keypoints   | Front view keypoints   | 
|:----|:----:|:----|:----:|
| 0. shoulder       1. left waist        2. left hip          3. right waist     4. right hip       5. ankle           | 0. crotch   1. left shoulder     2. left waist        3. left hip            4. left ankle  5. right shoulder  6. right waist  7. right hip  8. right ankle   | 

Because these are two-dimension figures, so we can directly describe the information of the key-points as in (x,y) format. The expected key-points structures are 18 (9x2) and 12 (6x2) of the front view and side view figure respectively. And the four files shown in figure1.2 are the target of the assignment. The .npy file contains the key-points array information of the body silhouette.

![图片](https://uploader.shimo.im/f/A5uuekQbkjERr6vS.png!thumbnail)


Figure 1.2 Collect the original figure then handle them as designed dataset 

### 1.2 Assignment 2

Based on the dataset from the TA, we know began to handle the data[The total amout of input data is 5.000.000, which was converted to binary by np.shape into 40.000.000 = 5.000.000x8 = 1000x200x200] in colab while the raw sources was mounted in google drive. 

At the begining, we need to handle all the raw figures into the same image sizes:  200x200. With the image and the matched key-points information, we also defined the draw function.

![图片](https://uploader.shimo.im/f/8nDkv2R3E9UxPDpB.png!thumbnail)

Figure 1.2 Collect the original figure then handle them as designed dataset 

Then we just used Pytorch to define, observe and test the MLP model and CNN model, which could constructed the key-points prediction model.

![图片](https://uploader.shimo.im/f/QFwMii6HAHQqrzxi.png!thumbnail)

Figure 1.3 MLP prediction model and error

![图片](https://uploader.shimo.im/f/3esoaDUm2B6Z3beu!thumbnail)

![图片](https://uploader.shimo.im/f/3erXzztheOqX9rLd!thumbnail)

Figure 1.4 CNN prediction model and error

### 1.3 Assignment 3

The assginment 3 is a feature engineering product, including clustering and pick up the extreme samples from the data set, which you could read the matched PDF file for further illtstration.

![图片](https://uploader.shimo.im/f/D2rytHucb0iiAiK3!thumbnail)

Figure 1.5 Conclusion of the Assignment 3 

### 1.4 Assignment 4

Assignment 4 is the image generation product, which I used a pretty tricky way to complete it, by switching the input size and output size to generate the predict model.

## Install

Just run these .ipynb files in [colab](https://colab.research.google.com/) as the order shows, then you could see the program effects.

## Content sequent

Assignment1 : Data collection,

Assignment2 : Prediction model test and comparing,

Assignment3 : Clustering and comparing the unsupervised learning methods.

Assignment4 : Prediction model of the key-points detection and image generation  


## Contributing

[@ypLIU-Alex]https://github.com/ypLIU-Alex

## License

MIT License
