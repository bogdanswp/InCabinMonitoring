In-Cabin Monitoring System Simulator
Introduction
This project is a software simulator for an in-cabin monitoring system. The simulator accepts video files as input, performs object detection and recognition on the video, and generates alerts based on defined rules.

The system is designed to simulate the operation of an in-cabin monitoring system as closely as possible, allowing for testing and development without the need for physical hardware.

Technologies
The simulator is written in C++ and uses OpenCV for computer vision tasks and TensorFlow for machine learning. The user interface is designed to be intuitive and easy to use, allowing users to upload videos, view processed video with object recognition overlays, and see the generated alerts.

Project Structure
The project is structured into several modules:

Data Processing: Processes video files, breaking them down into frames and preparing them for object detection and recognition.

Object Detection and Recognition: Implements object detection and recognition using OpenCV and TensorFlow. Pre-trained models are used for recognizing objects related to in-cabin monitoring, such as persons, mobile phones, seatbelts, etc.

Alert Generation: A rule-based system that generates alerts based on the objects detected and their state.

Interface: A user interface where users can interact with the system.

How to Build
This project uses CMake as a build system. The project includes a CMakeLists.txt file in the root directory, which you can use to build the project.

How to Contribute
Contributions are always welcome! Please feel free to submit a pull request or open an issue if you find a bug or think of a new feature that could be added.

Remember, this is just a template and should be customized based on your project's specifics. Good READMEs are very important as they are usually the first thing other developers will see when looking at your project. Make sure it accurately represents your project and provides the information that users or potential contributors will need.





