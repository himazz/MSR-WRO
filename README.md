# MSR-WRO

**Design Process of Self-Driving Car with Object Detection using YOLOv5 Model**

1. Introduction:
   This report presents the design process of a self-driving car equipped with an object detection system based on the YOLOv5 model. The car is intended for the World Robot Olympiad (WRO) competition. It comprises a rear driving motor and a steering motor, both controlled by an L298N motor driver. Additionally, the robot incorporates three Time-of-Flight (ToF) sensors connected to an Arduino via an I2C hub. The Arduino communicates with a Raspberry Pi 4, which deploys the trained YOLOv5 model for object detection. The development process involved data labeling and processing using Roboflow, and model training performed on Google Colab.

2. Requirements Analysis:
   The design process begins with a comprehensive analysis of the competition requirements and constraints. Size limitations, power source restrictions, weight restrictions, and specific rules set by the WRO competition are considered. These requirements guide the design and ensure compliance with the competition guidelines.

3. Mechanical Design:
   The mechanical design focuses on creating a sturdy and lightweight chassis that meets the size limitations specified by the competition. The chassis accommodates the rear driving motor and steering motor, ensuring proper alignment with the wheels. Ample space is provided to securely position the Arduino, Raspberry Pi, and other electronic components within the chassis.

4. Electrical Design:
   The electrical design involves establishing a reliable power supply system. The rear driving motor and steering motor are controlled using an L298N motor driver, which regulates the voltage and current supplied to the motors. The motor driver connects to the Arduino, which receives signals and commands from the Raspberry Pi for precise motor control. Interface protocols facilitate communication between the Arduino and Raspberry Pi.

   ![image](https://github.com/himazz/MSR-WRO/assets/25781254/d8f598c0-95a3-4491-8a60-ae132ad864fc)

   ![image](https://github.com/himazz/MSR-WRO/assets/25781254/1d44e867-7d2c-43f1-878f-8080bab962dd)



6. Sensor Integration:
   The self-driving car incorporates three ToF sensors placed in the front, right, and left directions. These sensors use infrared light to accurately measure the distance to nearby obstacles. Connected to an I2C hub, the sensors communicate with the Arduino simultaneously. The Arduino processes the sensor data, making informed decisions based on the detected obstacle distances. This integration enhances the car's autonomous navigation capabilities.

   

8. Object Detection Model Development:
   The object detection system is developed using the YOLOv5 model. Custom data labeling and processing are performed using Roboflow, which provides efficient annotation tools. The labeled dataset is prepared for training, ensuring sufficient diversity and quantity of annotated images. The training process utilizes Google Colab, a powerful cloud-based platform, to train the YOLOv5 model on the labeled dataset. The model is optimized for real-time object detection on the Raspberry Pi 4.

9. Software Integration:
   The trained YOLOv5 model is deployed on the Raspberry Pi 4, which is responsible for object detection. The Raspberry Pi processes the camera feed in real-time, identifying and localizing objects of interest within the car's surroundings. The detected objects are classified into predefined classes, enabling the self-driving car to make informed decisions based on the detected obstacles.

10. Testing and Calibration:
   Extensive testing and calibration are conducted to evaluate the performance of the self-driving car's object detection system. The car is tested in various scenarios resembling the competition environment, including different lighting conditions and obstacle configurations. Calibration ensures accurate distance measurements from the ToF sensors and precise object detection by the YOLOv5 model, enhancing the reliability and effectiveness of the self-driving car.

11. Optimization and Refinement:
   Based on the testing results, optimization and refinement are performed to enhance the performance of the self-driving car. This may involve fine-tuning the YOLOv5 model, adjusting sensor calibration parameters, optimizing power consumption, or improving the overall accuracy and speed of object detection. Iterative cycles of testing, analysis, and optimization are conducted until the self-driving car meets the desired performance standards.

12. Conclusion:
    The design process of the self-driving car with an object detection system based on the YOLOv5 model demonstrates the integration of mechanical, electrical, and software components. By combining the rear driving motor, steering motor, ToF sensors, Arduino, Raspberry Pi, and the YOLOv5 model, an autonomous vehicle capable of real-time object detection is developed. Thorough testing, calibration, and optimization contribute to achieving a high-performance self-driving car that can navigate obstacles effectively and meet the requirements of the WRO competition.
