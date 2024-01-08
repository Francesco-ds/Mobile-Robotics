## Table of contents
* [General info](#general-info)
* [Setup](#setup)
  
## General info
This project is simple A* implementation using potential field as heuristic
## Setup
To run this project:

- Set up the environment in unity the file can be found in the folder Unity (choose a scene)
- Set up the robot and goal and obstacles as you want (3 use cases can be found already in scene under test_potential_1/2/3 names)
    <p align="center">
  <img src="github_images/scene.jpg" alt="Scene" width="700">
</p>

- Open the A_star.py file and define start,goal coordinates
  <p align="center">
  <img src="github_images/start_and_goal.png" alt="Scene" width="700">
</p>

- Define obstacle data as your unity environment and run the code (x, x_scale, y, y_scale, flag). The flag is 0 if the obstacle is vertical (0 rotation), 1 if horizontal (90 degrees rotation in unity)
<div style="position: relative;">
  <img src="github_images/obstacle_data.png" width="500"  style="position: absolute; top: 50%; transform: translateY(-50%);" />
  <img src="github_images/obstacle_coordinates.jpg" width="400"  />
</div>

- You'll get printed on terminal the coordinates of your path, you'll also get in images the process visualized and a video showing the algorithm work

  <p align="center">


https://github.com/Francesco-ds/Mobile-Robotics/assets/58468024/03033d52-d1e0-4d0d-b62b-2937110783d1


</p>

- Copy the coordinates in a file.csv
- In the map_following.py change this line with the name of the csv you have created
    <p align="center">
  <img src="github_images/csv_path.png" alt="Scene" width="600">
</p>

-Run the scene on unity and run the map_following.py to see your robot moving

[new_use_case_1.webm](https://github.com/Francesco-ds/Mobile-Robotics/assets/58468024/42e7a908-bbd3-4a1c-90c8-7dd97dd6cd01)

