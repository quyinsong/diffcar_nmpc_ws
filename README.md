# diffcar_nmpc_ws  
基于NMPC的ROS无人车定点控制  
# main分支： 
main分支：在赵虚左老师搭建差速移动机器人的基础上实现NMPC控制  

# 安装
git clone https://github.com/quyinsong/diffcar_nmpc_ws.git  
# 测试  
终端输入  
cd ~/diffcar_nmpc_ws  
catkin_make  
source devel/setup.bash  
然后在另两个终端中分别输入：  
roslaunch mydiffcar_gazebo mydiffcar_gazebo.launch  
roslaunch nmpc_ctr nmpc_ctr.launch  
在rviz中发布2 D nav goal就可以完成小车的定点控制了  

![image](https://github.com/user-attachments/assets/034eec07-f8ff-4999-ba88-0a09da65dfd4)

# 问题
目前MPC没有加入任何障碍物约束，因此该项目暂不具备避障功能



