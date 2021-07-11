# human-tracking
This model takes a video and 2 line coordinates as input and return a json file with person id and time if he/she crosses the line. It also returns the images when line is crossed.
The model is trained on yolo v3 for object detection and deep sort for tracking.
Steps to run:
Download yolo weights from link: https://pjreddie.com/media/files/yolov3.weights  and place it in model_data folder.
Clone this repo.
Open terminal and change directory to cloned repo.
Run command "pip install -r requirements.txt"
Run command "python object_tracking.py"
On being asked, give location of video.
On beimg asked for coordinates, give input as x,y.
The output video will be saved as "track.mp4" and json file will be saved as "data.json"
An image folder will be created at same location which will contain all captured images.
Make sure to store output files or rename them otherwise they will be overwritten in next run.
