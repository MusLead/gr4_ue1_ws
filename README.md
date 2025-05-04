# 🤖 ROSY Description – Task A1.2

This ROS 2 project enables users to **visualize a robot model described in URDF** using **RViz2** and simulate its joint movements with the help of `joint_state_publisher_gui`.

---

## 📌 Prerequisites

This project is intended to be run on **Ubuntu Linux** (recommended version: **Ubuntu 22.04**) with **ROS 2 (Humble or later)** properly installed.

### ✅ Required ROS Packages

Before using this project, ensure the following ROS 2 packages are installed:

```bash
sudo apt update
sudo apt install -y \
  ros-humble-joint-state-publisher-gui \
  ros-humble-rviz2 \
  ros-humble-xacro
```

> 🧭 If ROS 2 is not installed, follow the official installation guide for your version at:
> [https://docs.ros.org/en/humble/Installation.html](https://docs.ros.org/en/humble/Installation.html)

---

## 🚀 How to Run the Visualization

1. **Clone the repository** (this repository *is* the workspace):

   ```bash
   git clone https://github.com/MusLead/gr4_ue1_ws.git
   cd rosy_ws
   ```

2. **Build the workspace**:

   ```bash
   colcon build
   ```

3. **Source the environment**:

   ```bash
   source install/setup.bash
   ```

4. **Launch the visualization (Task A1.2)**:

   ```bash
   ros2 launch rosy_description display.launch.py
   ```

---

## 🔍 What It Does

* Loads the robot URDF model in **RViz2**.
* Uses `joint_state_publisher_gui` to simulate the **rotation of the robot's wheel joints**.
* Ideal for inspecting robot design and motion before real-world deployment.

---

## 🛠️ How to Create a ROS 2 Package (for learning/reference)

To create a similar package manually, you may use:

```bash
ros2 pkg create rosy_description
```

> Replace `rosy_description` with your desired package name.

source: 
[Create and Set Up a ROS2 Workspace - ROS2 Tutorial 3](https://youtu.be/3GbrKQ7G2P0?si=4HON8bex9SfdtMYi)
[ROS2 - How to Publish TFs using URDF and Robot State Publisher](https://youtu.be/V_C8Cmv4fgk?si=esRdjgoOLAfIND1B)
[Create a URDF with ROS2 (1H Crash Course)](https://youtu.be/dZ_CyyEvBE0?si=rhyr0zifiNgdB4Ja)

