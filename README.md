# LINX (Line and Independant Navegation eXperiment)

![](./Assets/images/LINX_blck_21.png)

This project is a technology demontrator for semi guided navegation, in which we follow physical lines for part of the travel but can also move independantly using computer vision.

## How It Works

The web cams look for a line that they will use to locate thmeselves in space, they will also will be looking for ArUco markers which will indicate the robot where certain waypoints, obstacles and charging stations are located, it will proces this position and orientation data into the most optimal path that it can come up with and then it will send comands to the arduino for it to follow the desired path.

### Hardware:
- Arduino Mega 2560 board
- 10x CNY70 sensors
- HP laptop for image procesing
- Webcam
- ArUco Markers
  
### Software:
- Arduino IDE, Jetbrains Pycharm and VScode
- Python
  - OpenCV

## Project Structure

- ```deprecated```: Storage for old versions of the code, including FEM sensor guidance logic
- ```src```: The LTS version of the code, in which we are working
  - ```Arduino```
  - ```Q-Learning```
  - ```Machine Vision```

## Next Steps

Enhance Line-following on complex courses: Improve detection and handling of curves, intersections, and varying line widths.
Error handling: Incorporate fail-safes and recovery mechanisms for sensor malfunctions or unexpected scenarios.
User interface: We are considering adding a localy hosted webapp to be able to remotely call Linx.
Linx (FEM v2): We are currently developing a new version that incorporates machine vision to be able to navigate more complex terrain and go out of the line

### We welcome contributions to improve this project. Feel free to fork, submit pull requests, or raise issues.

- [@juanpanpanyz]( https://github.com/juanpanpanyz): - Juan Baader
- [@porfi2089](https://github.com/porfi2089): - Manuel Rao
- [@Defeeeee](https://github.com/Defeeeee): - Federico Diaz Nemeth
