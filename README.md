## Self-Driving Car with Object Detection using YOLOv5 Model

This repository contains the code and resources for a self-driving car equipped with an object detection system based on the YOLOv5 model. The car is specifically designed for the World Robot Olympiad (WRO) competition, offering autonomous navigation and obstacle detection capabilities.

### Features

- Utilizes a rear driving motor and a steering motor, controlled by an L298N motor driver.
- Incorporates three Time-of-Flight (ToF) sensors for accurate distance measurement to nearby obstacles.
- Deploys a Raspberry Pi 4 for real-time object detection using the trained YOLOv5 model.
- Supports custom data labeling and processing using Roboflow.
- Performs model training on Google Colab, ensuring optimized performance.

### Design Process

1. **Requirements Analysis**: Thoroughly analyze the WRO competition requirements and constraints to guide the design and ensure compliance.

2. **Mechanical Design**: Create a sturdy and lightweight chassis that accommodates the motors and electronic components while adhering to size limitations.

3. **Electrical Design**: Establish a reliable power supply system using the L298N motor driver for motor control and communication between the Arduino and Raspberry Pi.

4. **Sensor Integration**: Integrate three ToF sensors connected to an Arduino via an I2C hub for accurate distance measurement and obstacle detection.

5. **Object Detection Model Development**: Develop the object detection system using the YOLOv5 model and custom data labeling and processing using Roboflow.

6. **Software Integration**: Deploy the trained YOLOv5 model on the Raspberry Pi 4 to enable real-time object detection.

7. **Testing and Calibration**: Conduct extensive testing in various scenarios to evaluate the performance of the object detection system and calibrate the sensors and model.

8. **Optimization and Refinement**: Fine-tune the YOLOv5 model, adjust sensor calibration parameters, and optimize power consumption to enhance the self-driving car's performance.


9. **IMAGES AND VIDEOS**: The following section provides a reference for the PCB design and the provide useful videos 

    
**PCB Schematic** 

![image](https://github.com/himazz/MSR-WRO/assets/25781254/e03d8b80-4e92-4ac4-a098-40ac8c97a423)

**PCB Design** 

![image](https://github.com/himazz/MSR-WRO/assets/25781254/415ef6d8-9f6c-4095-b0d4-03b348a5d1ae)


**roboflow link** [https://app.roboflow.com/wro-pcq9c/boxfinder-gygic/deploy/1]

**YouTube Videos** 
1. object video for training [https://youtu.be/dY5cTE69LHM]
2. progress video [https://youtu.be/xcinS8bJSI8] 






### Usage

1. Clone the repository:
   ```
   git clone https://github.com/your-username/self-driving-car.git
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Prepare the dataset and perform data labeling using Roboflow.

4. Train the YOLOv5 model on Google Colab using the provided notebook.

5. Transfer the trained model to the Raspberry Pi 4.

6. Run the self-driving car code on the Raspberry Pi 4.

### Contributing

Contributions to this project are welcome. Feel free to submit issues, feature requests, and pull requests.

### License

This project is licensed under the [MIT License](LICENSE).

### Acknowledgments

We would like to acknowledge the contributions of the open-source community and the developers of YOLOv5, Roboflow, and Google Colab for their valuable tools and resources.

### References

- YOLOv5: [https://github.com/ultralytics/yolov5](https://github.com/ultralytics/yolov5)
- Roboflow: [https://roboflow.com](https://roboflow.com)
- Google Colab: [https://colab.research.google.com](https://colab.research.google.com)
