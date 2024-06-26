# Taiwan-Waste-Classifier
Using AI to Address Taiwan's Waste Classification &amp; Recycling Management

# Project Description
This project aims to develop an AI model tailored specifically for waste classification in Taiwan. Existing AI models from other countries often lack specificity for the unique types of waste commonly found in Taiwan and do not align with Taiwanese waste classification regulations. Taiwan’s recycling rate has reached an impressive 60% as of 2022, however, without a correct and precise classification at the source, recycled materials would be downgraded or treated as garbage upon reaching recycling plants. 
To address this issue, we have curated a comprehensive dataset composed of images of various waste items collected in Taipei, and combined with other external sources. Our AI model will accurately identify and classify the different types of waste found in Taiwan, providing clear instructions on their appropriate disposal methods.

# Getting Started
[Taiwan Waste Dataset](https://drive.google.com/drive/folders/1-1xCiUErjF-nEyUobdbqsEdGfIY-ZnoZ?usp=drive_link)



# File Structure
Total: 5112 (contains 6 classes)<br/><br/>

* General (一般垃圾): 501<br/>
* General Recycle (一般資源回收): 1398<br/>
* Styrofoam (保麗龍): 496<br/>
* Plastic Bag (塑膠袋): 376<br/>
* Paper (廢紙): 1300<br/>
* Paper Container (紙容器): 468<br/>


# Analysis
To address the specific needs of waste classification in Taiwan, we employed a convolutional neural network (CNN) architecture. The key steps in our analysis included:<br/>
* Data Collection and Preprocessing: We collected images of waste from various sources, focusing on six categories of garbage in Taiwan: cardboard, glass, metal, paper, plastic, and trash. Each image was resized to 32x32 pixels and converted to tensors for neural network processing.<br/>
* Model Architecture: We built a CNN using the Sequential API in Keras. The model included convolutional layers to extract features from the images, pooling layers to reduce spatial dimensions, and fully connected layers to perform the final classification. A softmax activation function was applied in the output layer to produce probability scores for each category.<br/>
* Training and Evaluation: The model was trained on a dataset split into training and validation sets. Metrics such as test accuracy, test loss, and the confusion matrix were used to evaluate the model.<br/><br/>
From our analysis, we gained several key insights:<br/>
* Model Accuracy: The final test accuracy of 72.21% demonstrates that our model performs well in classifying various types of waste according to Taiwan's specific categories. This high level of accuracy indicates that the model can effectively support waste sorting processes.<br/>
* Error Analysis: The confusion matrix and classification report highlighted specific categories where the model performed exceptionally well, such as general recycling, styrofoam, and plastic bags. However, it also revealed areas where improvements are needed.<br/>

# Results
The developed AI model tailored for waste classification in Taiwan achieved a final test accuracy of 72.21% and test loss of 1.36, demonstrating great performance on unseen data. The model excels in predicting categories like general recycling, styrofoam, and plastic bags while maintaining high accuracy across other waste types. For each input waste image, the model provides the classified label (e.g., Trash, Recyclable - Paper) and a recommendation on the appropriate disposal method and collection schedule.<br/><br/>
By enabling precise waste classification at the source, the model addresses Taiwan's need for accurate identification aligned with local waste types and regulations. This can prevent the downgrading of recyclable materials and ensure proper recycling practices, leading to an increase in recycling rates, reduction in landfill use, and lower processing costs at recycling facilities, contributing to Taiwan's environmental sustainability and circular economy efforts.<br/><br/>
Future work could involve expanding the dataset and categories, refining performance for lower-accuracy categories, and integrating the model into existing waste management systems or user-friendly applications to facilitate broader adoption and impact for all residents in Taiwan. 

# Contributors
謝宜蓁 Coding, project discussion<br/>
鄒宸萱 Coding, project discussion, project presentation <br/>
韋欣 Dataset collection, project methodology discussion, booth poster design <br/>
胡裔婕 Project ideation, dataset collection, slide design <br/>
李聖悅 Dataset collection, project methodology discussion, project presentation <br/>
葉可彤 Dataset collection <br/>

# Acknowledgments
We would like to express our sincere gratitude to the following individuals for their invaluable contributions to this project:<br/><br/>
Pien, Chung-Pei (Professor): We are deeply grateful to professor Pien for providing guidance and mentorship throughout the project. Your expertise and insights were instrumental in shaping our approach and ensuring the success of this project.<br/><br/>
Ian Huang (Teaching Assistant): We are very grateful to Ian for his unwavering support and guidance throughout the coding process. <br/><br/>
The Kaggle Community: We would like to acknowledge the open-source community and the valuable resources they have created, which served as the foundation for our work. Specifically, we utilized some datasets from other creators for an increased accuracy. 

# References
Dataset sources (for non-Taiwanese trash):<br/>
https://www.kaggle.com/datasets/mostafaabla/garbage-classification<br/>
https://www.kaggle.com/datasets/ashwinshrivastav/most-common-recyclable-and-nonrecyclable-objects<br/>
https://www.kaggle.com/code/farzadnekouei/imbalanced-garbage-classification-resnet50<br/>
https://www.kaggle.com/datasets/mostafaabla/garbage-classification<br/><br/>


Other Market Research sources:<br/>
https://news.pts.org.tw/article/488630<br/>
https://www.nyckel.com/pretrained-classifiers/recycling-identifier/<br/>
https://www.taiwanwatch.org.tw/node/1385<br/>
