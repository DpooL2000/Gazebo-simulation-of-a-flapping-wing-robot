# Gazebo-simulation-of-a-flapping-wing-robot

This repository contains the code for a flight simulation project designed to analyze and control a simulated bird using ROS 1 with Gazebo. The project includes GUI components for real-time control and data visualization, as well as various controllers and plugins for simulating and analyzing bird flight dynamics.

![model](image.png)

https://github.com/user-attachments/assets/a7cf18eb-7885-481c-bfef-dfd814341838

https://github.com/user-attachments/assets/d4963d1c-1f1d-4fe9-a71b-3e7e6bd960d6

## File Structure

- **`CMakeLists.txt`**: Build configuration file for CMake.
- **`package.xml`**: ROS package configuration file.
- **`launch/`**: Launch files for ROS.
  - `simple.launch`: Launch file to start the simulation.
- **`models/`**: Gazebo models used in the simulation.
  - `bird2/`: Directory containing the bird model.
- **`src/`**: Source files and UI files.
  - `flapping_controller.cpp`: Implementation of the flapping controller.
  - `flight_controller_gui.cpp`: Implementation of the GUI.
  - `lift_drag_plugin.cpp`: Implementation of the lift and drag plugin.
  - `pitching_controller.cpp`: Implementation of the pitching controller.
  - `rolling_controller.cpp`: Implementation of the rolling controller.
  - `test1.ui`: UI design file.
- **`worlds/`**: Gazebo world files.
  - `simple.world`: World file for the simulation.

## Getting Started

1. **Clone the repository:**
   Navigate to the root directory and use CMake to configure and build the project:
   ```bash
   git clone https://github.com/yourusername/your-repository.git
   
2. **Build the Project:**
   You can start the simulation with the provided launch file:
   ```bash
    cd your-repository
    mkdir build
    cd build
    cmake ..
    make

4. **Launch the Simulation:**
   ```bash
   roslaunch your_package_name simple.launch

5. **Launch the Simulation controller GUI:**
   ```bash
   rosrun your_package_name flight_ontroller_gui.cpp

## Features

- **GUI Controls:** Interface for real-time control of the simulation parameters.
- **Data Visualization:** Tools for visualizing flight data in real-time.
- **ROS Integration:** Interfaces with ROS for communication and control.
- **Gazebo Simulation:** High-fidelity simulation of bird flight dynamics.

## Contributing

Feel free to contribute to the project by submitting issues or pull requests.

## License

This project is licensed under the Apache License. See the LICENSE file for details.
