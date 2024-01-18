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
  ```
  start_and_goal = [(start_x,start_y),(goal_x,goal_y)]
  ```

- Define obstacle data as your unity environment and run the code (x, x_scale, y, y_scale, flag). The flag is 0 if the obstacle is vertical (0 rotation), 1 if horizontal (90 degrees rotation in unity)

  <p align="center">
  <img src="github_images/obstacle_coordinates.jpg" width="400"  />
  </p>
  
   ```
  obstacle_data = [(obstacle_x,obstacle_x_scale,obstacle_y,obstacle_y_scale,flag)]
  ```

  


- You'll get printed on terminal the coordinates of your path, you'll also get in images the process visualized and a video showing the algorithm work

  <p align="center">


https://github.com/Francesco-ds/Mobile-Robotics/assets/58468024/03033d52-d1e0-4d0d-b62b-2937110783d1


</p>

- Copy the coordinates in a file.csv
- In the map_following.py change this line with the name of the csv you have created

  ```
  self.csv_file_path = path_name
  ```
  
- Run the scene on unity and run the map_following.py to see your robot moving (video is sped up)

 

https://github.com/Francesco-ds/Mobile-Robotics/assets/58468024/fc15cbbf-8ddd-4368-9682-fef73040a6be



- Case 2:
  
Path to follow:


https://github.com/Francesco-ds/Mobile-Robotics/assets/58468024/fea2e2bc-6205-48f9-a5a7-fe92a69bc079


Sped up video:



https://github.com/Francesco-ds/Mobile-Robotics/assets/58468024/b3e7932a-74fd-4c69-a679-a1f62b055453


- Case 3

Path to follow


https://github.com/Francesco-ds/Mobile-Robotics/assets/58468024/6b2b8882-0671-4e78-acc1-59ce1b709ee7

Sped up video:



https://github.com/Francesco-ds/Mobile-Robotics/assets/58468024/0a851f77-ce79-438e-add8-f62871ae9af3




