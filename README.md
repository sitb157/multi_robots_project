# Mulit robots project

### Test world!!
<img width="802" alt="world_sample" src="https://github.com/sitb157/multi_robots_project/assets/108820413/6f2c17a5-d984-4678-9ced-4a371c52cb46"></br>

#### Run  
```bash    
git clone --recursive https://github.com/sitb157/multi_robots_project.git  
```  
```bash
cd docker/
```
```bash
docker-compose up --build
```
##### start robots container to run gazebo
```bash
./exec_robots.sh
```
```bash
(robots container) colcon build
```
```bash
(robots container) ros2 launch gz_worlds gz_worlds.launch.py
```

##### start naviagion container to run navigation
```bash
./exec_navigation.sh
```
```bash
(navigation container) colcon build
```
```bash
(navigation container) ros2 launch navigation navigation2.launch.py
```
