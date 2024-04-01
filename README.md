
# Summary
This repository contains the code to run and deploy an embedded machine learning program (TinyML) on an embedded system (e.g. Arduino, Raspberry PI, ESP32).
More specifically, this is a computer vision model that is used to identify clothing types. These detections are then used to determine what sequence of joint movements are needed to fold the garments.

It was trained and optimized using Edge Impulse to leverage edge computing with quantization. INT8 data is used as an alternative to FP32 to increase effeciency and overcome the storage concerns of using a microprocessor. A USB webcam is used to obtain real-time visuals. 

Through deployment, the model can be run locally on the microcontroller/microprocessor, meaning a network connection will not be necessary to use the model. Note that both a 64-bit OS and 64-bit CPU on the embedded system are necessary for deployment.

# Usage

Deploy as a C++ library: https://docs.edgeimpulse.com/docs/deploy-your-model-as-a-c-library

Running locally: https://docs.edgeimpulse.com/docs/running-your-impulse-locally-1

# Examples

![](https://cdn.discordapp.com/attachments/928022919337103393/1210464639155183626/Screenshot_2024-02-23_005413.jpg?ex=65fd1d0b&is=65eaa80b&hm=70eafbad6b086c4e97d6a764c09339e78f23d931fbb715e0502eb2f0b8576e49&)

![](https://cdn.discordapp.com/attachments/928022919337103393/1210465112176066590/Screenshot_2024-02-23_005604.jpg?ex=65fd1d7c&is=65eaa87c&hm=14a2588dcc9fc03307f30e46263e16ed96cb9266765359f44285cf154cf8014c&)

**Note for pants, that the `top` and `bottom` parts had to be identified for accurate folding. A shirt is simply denoted as `shirt`.**



