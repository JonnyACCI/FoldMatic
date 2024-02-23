
# Summary
This repository contains the code to run and deploy an embedded machine learning program (TinyML) on an embedded system (e.g. Arduino, Raspberry PI, ESP32).
More specifically, this is a computer vision model that is used to identify clothing types. These detections are then used to determine what sequence of joint movements are needed to fold the garments.

It was trained and optimized using Edge Impulse to leverage edge computing with quantization. INT8 data is used as an alternative to FP32 to increase effeciency and overcome the storage concerns of using a microprocessor. A USB webcam is used to obtain real-time visuals. 

Through deployment, the model can be run locally on the microcontroller/microprocessor, meaning a network connection will not be necessary to use the model. Note that both a 64-bit OS and 64-bit CPU on the embedded system are necessary for deployment.

# Usage

Deploy as a C++ library: https://docs.edgeimpulse.com/docs/deploy-your-model-as-a-c-library

Running locally: https://docs.edgeimpulse.com/docs/running-your-impulse-locally-1

# Examples

![](https://media.discordapp.net/attachments/928022919337103393/1210464639155183626/Screenshot_2024-02-23_005413.jpg?ex=65eaa80b&is=65d8330b&hm=c9e6307712b382de452b85bf028e704d9e8d3f804d2d4d8177f7dcb87a9740d8&=&format=webp&width=567&height=733)

![](https://cdn.discordapp.com/attachments/928022919337103393/1210465112176066590/Screenshot_2024-02-23_005604.jpg?ex=65eaa87c&is=65d8337c&hm=2b3c362555b4cc2a146eff7cca7e4e9fa154a10bbaa1fe725db34648bed6dcc1&)

**Note for pants, that the `top` and `bottom` parts had to be identified for accurate folding. A shirt is simply denoted as `shirt`.**



