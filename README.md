# Attentional Visual Field (AVF) Task

Traditionally, an Attentional Visual Field task is developed for and conducted on a desktop computer. While completing this task, participants are instructed to keep their heads in a chinrest to ensure that the visual stimuli are displayed at the appropriate size and distance. Participants must also fixate on a central point on the screen around which the other visual stimuli are calibrated to be at certain distances from the center of the visual field. This task measures the spread of attention across the visual field by displaying targets at different locations in the visual field based on the target's direction and distance from the center of the visual field. Participants are instructed to indicate which direction the target appears in for each trial, and their accuracy and response time are used to describe the shape of their attentional visual field.
<br>
<br>
# XR Attentional Visual Field Task

This XR Attentional Visual Field Task is based on the computer-based AVF task. It has been developed to work with most VR and AR headsets by implementing the OpenXR API within the Unity3D game engine. This project uses Unity version 2020.3.7f1. 
<br>
<br>

# Getting Started

1. Install Unity version 2020.3.7f1 if it is not already present on your device to ensure the project works as intended.

2. Download the zip folder with all of the required files for Unity. 

3. Extract the files from the zip folder and add the project folder titled "XR AVF" as a new project through the Unity Hub.

4. Launch the project through the Unity Hub.

5. Add any assets necessary for your experiment to the TaskRoom scene. This could include things such as, a virtual environment, virtual objects, eye-tracking add-ons, etc.

6. Modify the experiment settings on the Experiment Settings object located in the InfoScreen scene.
<br>
<br>

# Explanation of Experiment Settings
![Exp Settings](https://user-images.githubusercontent.com/105318271/177431751-725002e8-59d5-478c-ad72-bf67ff205285.png)
Setting | Description
------------ | -------------
Num Of Blocks | Determines how many blocks the experiment will have.
Target Visual Angle | The size of the target stimulus in the number of degrees in visual angle.
Distractor Visual Angle | The size of the distractor stimuli in the number of degrees in visual angle.
Eccentricities | The number of locations in each direction that a target will appear in. Expand this list to set the individual eccentricity values to control exactly where the stimuli will appear in the number of degrees in visual angle.
Exposure Times | The number of different display times that each target will appear for. Expand this list to set the individual exposure time values to control exactly how long the target stimulus will be visible for in each trial in seconds. Example values include .04, .06, .10. These values would represent 40, 60, and 100 ms, respectively.
Trial Repetitions | Determines how many times each unique trial will be presented in each block. A unique trial is comprised of an eccentricity, an exposure time, and a direction within the visual field. Stimuli will appear in 8 different directions in any iteration of this experiment as it is based on the computer AVF task. In this example image, there would be 72 unique trials (8 directions x 3 eccentricities x 3 exposure times) per block. 2 trial repetitions would lead to there being 144 total trials in the experiment.
