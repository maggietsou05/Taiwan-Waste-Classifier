# Taiwan-Waste-Classifier
Using AI to Address Taiwan's Waste Classification &amp; Recycling Management

# Project Description
This project aims to develop an AI model tailored specifically for waste classification in Taiwan. Existing AI models from other countries often lack specificity for the unique types of waste commonly found in Taiwan and do not align with Taiwanese waste classification regulations. Taiwan’s recycling rate has reached an impressive 60% as of 2022, however, without a correct and precise classification at the source, recycled materials would be downgraded or treated as garbage upon reaching recycling plants. 
To address this issue, we have curated a comprehensive dataset composed of images of various waste items collected in Taipei, and combined with other external sources. Our AI model will accurately identify and classify the different types of waste found in Taiwan, providing clear instructions on their appropriate disposal methods.

# Getting Started




# File Structure




# Analysis
To address the specific needs of waste classification in Taiwan, we employed a convolutional neural network (CNN) architecture. The key steps in our analysis included:
Data Collection and Preprocessing: We collected images of waste from various sources, focusing on six categories of garbage in Taiwan: cardboard, glass, metal, paper, plastic, and trash. Each image was resized to 32x32 pixels and converted to tensors for neural network processing.
Model Architecture: We built a CNN using the Sequential API in Keras. The model included convolutional layers to extract features from the images, pooling layers to reduce spatial dimensions, and fully connected layers to perform the final classification. A softmax activation function was applied in the output layer to produce probability scores for each category.
Training and Evaluation: The model was trained on a dataset split into training and validation sets. Metrics such as test accuracy, test loss, and the confusion matrix were used to evaluate the model.
From our analysis, we gained several key insights:
Model Accuracy: The final test accuracy of 72.21% demonstrates that our model performs well in classifying various types of waste according to Taiwan's specific categories. This high level of accuracy indicates that the model can effectively support waste sorting processes.
Error Analysis: The confusion matrix and classification report highlighted specific categories where the model performed exceptionally well, such as general recycling, styrofoam, and plastic bags. However, it also revealed areas where improvements are needed.

# Results
The developed AI model tailored for waste classification in Taiwan achieved a final test accuracy of 72.21% and test loss of 1.36, demonstrating great performance on unseen data. The model excels in predicting categories like general recycling, styrofoam, and plastic bags while maintaining high accuracy across other waste types. For each input waste image, the model provides the classified label (e.g., Trash, Recyclable - Paper) and a recommendation on the appropriate disposal method and collection schedule.
By enabling precise waste classification at the source, the model addresses Taiwan's need for accurate identification aligned with local waste types and regulations. This can prevent the downgrading of recyclable materials and ensure proper recycling practices, leading to an increase in recycling rates, reduction in landfill use, and lower processing costs at recycling facilities, contributing to Taiwan's environmental sustainability and circular economy efforts.
Future work could involve expanding the dataset and categories, refining performance for lower-accuracy categories, and integrating the model into existing waste management systems or user-friendly applications to facilitate broader adoption and impact for all residents in Taiwan. 

# Contributors
謝宜蓁 <br/>
鄒宸萱 <br/>
韋欣 Dataset collection, project methodology discussion, booth poster design <br/>
胡裔婕 Project ideation, dataset collection, presentation slide design <br/>
李聖悅 Dataset collection, project methodology discussion, project presentation <br/>
葉可彤 Dataset collection <br/>

# Acknowledgments
We would like to express our sincere gratitude to the following individuals for their invaluable contributions to this project:
Pien, Chung-Pei (Professor): We are deeply grateful to professor Pien for providing guidance and mentorship throughout the project. Your expertise and insights were instrumental in shaping our approach and ensuring the success of this project.
Ian Huang (Teaching Assistant): We are very grateful to Ian for his unwavering support and guidance throughout the coding process. 
The Kaggle Community: We would like to acknowledge the open-source community and the valuable resources they have created, which served as the foundation for our work. Specifically, we utilized some datasets from other creators for an increased accuracy. 
