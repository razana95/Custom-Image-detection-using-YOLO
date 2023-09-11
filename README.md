# Custom-Image-detection-using-YOLO
WORKFLOW

1)Dataset Inspection:

Analyze the provided dataset, including images and XML annotation files.

Identify any inconsistencies or missing annotations.

2)Removing Unannotated Images:

Remove images without corresponding annotated XML files to ensure data consistency.

3)XML to TXT Conversion:

Convert XML annotation files to YOLOv8-compatible TXT format.

Extract three class of vehicles namely rickshaw,three wheelers(CNG) and minivan and their IDs, object coordinates (center_x, center_y, width, height).

4)Splitting Dataset:

Divide the dataset into training, validation, and test sets.

Maintain the proper balance of data in each split.

4)Creating Data.yaml File:

Generate a data.yaml file specifying:

Paths to training, validation, and test data folders.

Number of classes (3: rickshaw, three wheelers (CNG), minivan).

Class labels (names).

5)Model Training (YOLOv8):

Utilize a pre-trained YOLOv8 model.Yolov8 is pre trained with 4 vehicle classes namely car,bus,truck and motorcycle.

Fine-tune the model on my custom dataset with the specified classes.(rickshaw,three wheelers(CNG) and minivan)

Train the model for object detection.

6)Inference:

Use the trained model to make predictions on new or test images.

Obtain bounding box coordinates and class predictions.
