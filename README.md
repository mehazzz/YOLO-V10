# YOLO-V10
An AI model which identifies and helps in segregation of waste in day to day life with the help of YOLO V10
Steps for the multi object detection model
Implementation of the waste management system was primarily done in three components: data 
collection, training the model, and testing/evaluation. 
1. Dataset Collection and Annotation 
A comprehensive dataset was gathered using Roboflow as the foundation for the project. It 
consisted of images of various trash objects, which were systematically annotated and categorized 
into three primary classes: recyclable, biodegradable, and non-biodegradable. This was defined by 
three primary categories: - Recyclable: These are items that can be processed and reused, such as plastics, glass, and metals. - Biodegradable: Organic waste made of food remnants and paper that can decompose naturally. - Non-biodegradable: Materials that do not break down easily and are largely non-recyclable, 
including specific plastics and synthetic fibers. 
To ensure the robustness of the dataset, images were collected from multiple sources, 
encompassing various conditions and angles. 
2. Data Annotation 
Immediately after the collection, images were carefully annotated. Every picture had its category 
labeled on it. This was one important process for the correctness of the YOLO model. Challenges 
in annotation are usually seen in cases like materials that look alike, and mixed waste images 
requiring careful segmentation to categorize each item accordingly. 
3. YOLO v10 Model Architecture 
The YOLO v10 model was used mainly because of its improved architecture, which includes using 
a convolutional layer on the input images to scan to extract all features and proceed with further 
detection layers in calculating the bounding boxes as well as identifying the objects detected. On 
waste segregation, this specific architecture is effective since images process fast and effectively. 
4. Model Training 
The training of the YOLO v10 model was done using the Ultralytics package. Preliminary 
experiments used cross-validation to settle optimal batch size and epochs to arrive at better values 
for this model. Its hyperparameter tuning was used, tuning learning rate, batch size, and number 
of epochs to further advance the effect of the model. 
The data augmentation techniques were utilized to increase the capacity of the model by giving 
other forms of the training image so that overfitting wouldn't occur. A flowchart was designed to 
highlight the pipeline of training; it was a representation of everything, from inputting of data to 
the output made by the model. 
5. Evaluation and Performance Metrics 
The performance of the YOLO v10 model was evaluated based on precision, recall, and mean 
average precision (mAP). These were measured by running the model's predictions against a 
validation set so that its ability to correctly classify various types of waste can be fully determined.

