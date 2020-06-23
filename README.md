# INTELLIGENT TRAFFIC MONITORING SYSTEM[README]

OpenCV image filters.
Object detection by contours.
Building processing pipeline for further data manipulation.

## Problem Statement
Develop an inteligent traffic monitoring system which can control traffic lights based on number of vehicles in roads

## Project in a nutshell
<ul>
  <li>
    Uses Computer Vision to identify number of vehicle in a road and adjust the time of changing of traffic light accordingly
  </li>
  <li>
    Using MOG algorithm, CC camera in traffic post
  </li>
  <li>
    Main Tools Used: OpenCV, SK-Video, MySQL
  </li>
</ul>

## Solution in Detail
<ul>
<li>
MOG Algorithm - For background subtraction
</li>
<li>
Foreground_objects = current_frame - background_layer
<li>
Filtering
Removing unwanted noises to make the object look bolder
</li>
<li>
Object detection by contours
we will use the standard cv2.findContours method
</li>

<li>
So we created contour detection first just merged together out bg subtraction filtering and detection parts
</li>
<li>
Created a processor that will link detected objects on different frames and will create paths, and also will count vehicles.
</li>
<li>
The vehicles entering and exiting the detection zone will be counted and the number of vehicles in the in-zone is obtained
</li>

<li>
The number of vehicles inside each of the lane is used to decide the current and the upcoming traffic lights.
</li>

<li>
We are following a Round robin based distribution of the cycle to the lanes
and our algorithm could be easily mapped for junctions with varying number of intersecting roads.
</li>

</ul>
<!--
The recorded cc cam data is also used for a variety of other use cases like 
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






