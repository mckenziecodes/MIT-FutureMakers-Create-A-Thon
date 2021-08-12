# MIT-FutureMakers-Create-A-Thon
This repository contains the code and information for the Create-A-Thon portion of the MIT FutureMakers program (Team 10).

Team #10 - dooDLers
Prompt #2 - Climate Change and Environmental Risk Mitigation
Project - SmartSaver

# What is SmartSaver?
SmartSaver uses smart technology to minimize energy waste and add transparency to help people make smart decisions. 

# Why do we need SmartSaver?
Many of us are concerned about climate change and COVID-19. People are trying to minimize their climate footprints and still want to leave their homes. As of now, there isn’t much transparency in public places. If you want to work in a library, you have to worry about which places are safe to sit, for example.

# Focus.
Our primary focus is climate change, a massive and complex issue. Many people claim they want to do something for the environment, but they can’t or won’t put these ideas into practice. What people need is a way to implement sustainability into their everyday lives without having to think about it on a daily basis.

# How does it work?
SmartSaver is for smart building design. It saves energy by determining whether or not to turn off amenities such as lighting, HVAC systems, or ventilation; based on whether an area or a room is occupied at that time or not.

As our system bases its decisions based in part on the occupancy of a room or table, it can also be used to help determine which areas in a public location (such as an office or restaurant) are safe for people to use.

Our product has sensors, which we will talk about shortly. Those sensor readings are fed into a deep learning model to predict which system should stay on and which system would save energy by getting shut off for a while. 

While our solution’s main aim is to save energy by controlling the power usage as per the building’s and occupant’s requirement, which would also control greenhouse gas emission as a part of controlling HVAC system running times… we want to expand our solution to one of the most pressing matter of the last couple of years, which is COVID-19. Our system can detect which public desk/table is safe to sit at, by keeping track of the duration some previous person was sitting there.

# Who can use SmartSaver?
Our product can be implemented in all sorts of public spaces, including offices, restaurants, schools, recreational centers, nursing homes, and libraries. Thus, people who manage these spaces would profit greatly from our technology. This includes city managers, urban planners, businesspeople, and restaurant owners. 

Additionally, anyone who uses these spaces would benefit as well. And finally, if SmartSaver is implemented in homes, any homeowner can enjoy both the reduced energy usage and the extra measures to be safe from COVID-19. As a result, most everyone can be a beneficiary of SmartSaver.

# Technicalities.
We aimed to build something that’s non-intrusive and doesn’t prompt people to  perform actions. So, we used sensors that take non-visual, data. Our small silicon chips are incredibly easy to install in a room. 

From 5 sensors, we gathered motion, temperature, humidity, luminosity, and CO2 data. We found a dataset from the UCI Machine Learning repository, which served our needs well (especially in terms of sample count and granularity of the data). 

We performed research on that dataset and used a fully connected neural network as our baseline. Originally, it had 92.42% accuracy, but we improved it to gain a 98.91% accuracy. 

We fed our neural network normalized data and performed correlation analysis (to see which sensors are performing in tandem). We used this information to predict the length of occupancy of for a certain room or table. 
