## streaming-05-smart-smoker\
#Creating a Producer

Streaming data may come from web analytics, social media, smart devices, and more. In these next two modules, we'll look at implementing analytics for a "smart smoker" (as in slow cooked food). 

In Module 5, we'll understand the process, design our system, and implement the producer. 

The Problem / Challenge To Solve
Please read about the Smart Smoker system here: Smart Smoker
Access the smoker data file here Download smoker data file here.
We want to stream information from a smart smoker. Read one value every half minute. (sleep_secs = 30)

smoker-temps.csv has 4 columns:

[0] Time = Date-time stamp for the sensor reading
[1] Channel1 = Smoker Temp --> send to message queue "01-smoker"
[2] Channel2 = Food A Temp --> send to message queue "02-food-A"
[3] Channel3 = Food B Temp --> send to message queue "03-food-B"
Requirements

RabbitMQ server running
pika installed in your active environment
RabbitMQ Admin

Image showing initial message asking if I'd like to launch Rabbit MQ
<img width="960" alt="mod 5 1" src="https://github.com/DrSTaylor/streaming-05-smart-smoker/assets/105294873/4fc4f654-384b-4479-b924-8f6d809c7fde">

Image showing Rabbit MQ which opened
<img width="960" alt="mod 5 2" src="https://github.com/DrSTaylor/streaming-05-smart-smoker/assets/105294873/042bc8c7-5060-4d31-b0e6-4db2660eca52">

Image showing producer sending the message at regular intervals

<img width="960" alt="mod 5 3" src="https://github.com/DrSTaylor/streaming-05-smart-smoker/assets/105294873/1a568b68-b9b2-4f44-8d6e-192bd8951131">
