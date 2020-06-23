# INTELLIGENT TRAFFIC MONITORING SYSTEM[README]

OpenCV image filters.
Object detection by contours.
Building processing pipeline for further data manipulation.

<!--

MOG Algorithm - For background subtraction
foreground_objects = current_frame - background_layer

Filtering
Removing unwanted noises to make the object look bolder

Object detection by contours
we will use the standard cv2.findContours method


Building processing pipeline
So we create contour detection first, o just merge together out bg subtraction, filtering and detection parts.
Now let’s create a processor that will link detected objects on different frames and will create paths, and also will count vehicles.
The vehicles entering and exiting the detection zone will be counted and the number of vehicles in the zone is obtained



The number of vehicles inside each of the lane is used to decide the current and the upcoming traffic lights.

We are following a Round robin based distribution of the cycle to the lanes
and our algorithm could be easily mapped for junctions with varying number of intersecting roads.

The recorded cctv data is also used for a variety of other use cases like 
pedestrian detection and signal allocation for pedestrians
Vehicle classifier and then intelligently map the duration
Number plate detection and other traffic rule violations.
-->
References:

Object detection
https://opencv.org/

Vehicle count collection:
github.com/creotiv/object_detection_projects

Mysql Database connections:
https://www.journaldev.com/15539/python-mysql-example-tutorial






