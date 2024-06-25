# UML diagram visualization in Visual Studio of local PC 

This document utilizes PlantUML and Marker Kroki for diagram visualization directly within the README.md file using Visual Studio Code in your local PC. 

## Prerequisites

1. **Visual Studio Code**: Ensure you have Visual Studio Code installed on your machine. You can download it from [here](https://code.visualstudio.com/).

2. **PlantUML Extension**: Install the PlantUML extension for Visual Studio Code. You can find it in the extensions marketplace or install it directly from [here](https://marketplace.visualstudio.com/items?itemName=jebbs.plantuml).

3. **Marker Kroki Extension**: Install the Marker Kroki extension for Visual Studio Code. You can find it in the extensions marketplace or install it directly from [here](https://marketplace.visualstudio.com/items?itemName=pomdtr.markdown-kroki).

## Setup Instructions

### 1. Install PlantUML Extension

- Open Visual Studio Code.
- Go to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window or press `Ctrl+Shift+X`.
- Search for "PlantUML" and install the extension by jebbs.

### 2. Install Marker Kroki Extension

- In the Extensions view, search for "Marker Kroki" and install the extension by mieubrisse.

### 3. Configure and Use PlantUML

- Inside your README.md file, you can add PlantUML diagrams using the following syntax:

  ```c4plantuml
  @startuml
  
  // Your UML diagram code here
  
  @enduml

### 4. Preview the Diagram
- To preview the diagram within the README.md file, press Ctrl+Shift+V or right-click on the file and select "Preview".
- You should be able to see the UML diagrams rendered directly in the preview pane of your README.md file.


# Example Diagram
#
Here’s an example of how to use UML desing and review the diagram in your README.md:
#


 ```c4plantuml
@startuml
|Data Preparation|
start
:Prepare Dataset in docker ig., /app/dataset Folder;
:Define Custom Dataset Class;
:Load Dataset (Images, Numpy Arrays, Excel Files);
:Transform Data Using torchvision.transforms.ToTensor;

|Model Preparation|
:Load Pre-trained Faster R-CNN Model (ResNet-50 FPN);

|Model Customization|
:Modify Classifier Head for 2 Classes;

|Training|
:Define Training Parameters (Optimizer, Scheduler);
:Train Model for 10 Epochs;
:Handle Batch Errors During Training;

|Saving and Conversion|
:Save Trained Model Checkpoint (model.pt);
:Convert Model to ONNX Format (model.onnx);

stop
@enduml
 ```


#

#
### Author

- Jimmy Majumder
- Robotics Software Enginner,
- Development_Team
- QibiTech Inc., Japan
- j.majumder@qibitech.com
