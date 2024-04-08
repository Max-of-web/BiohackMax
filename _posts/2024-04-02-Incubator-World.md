---
layout: post
title: Building an AI-Integrated Mushroom Incubator
date: 2024-03-25
permalink: /Building-an-AI-Integrated-Mushroom-Incubator/ # Change this to the desired URL
---

The **TastyMushroomIncubator** project is an ambitious endeavor to create a sophisticated mushroom incubator. The project is planned in three stages, evolving from a miniature prototype to a full-size, AI-powered environmental control system.

## Table of Contents

- [Introduction](#introduction)
- [Project Stages](#project-stages)
  - [Stage 1: Miniature Mushroom Incubator Design and Assembly](#stage-1-miniature-mushroom-incubator-design-and-assembly)
  - [Stage 2: Full-Size Incubator / Plant Grower](#stage-2-full-size-incubator--plant-grower)
  - [Stage 3: AI Integration for Automated Environmental Control](#stage-3-ai-integration-for-automated-environmental-control)
- [Inspiration](#inspiration)
- [Implementation and Testing](#implementation-and-testing)
- [Project Progress](#progression)
- [Conclusion](#conclusion)

## Project Stages

### Stage 1: Miniature Mushroom Incubator Design and Assembly

- **Materials and Components:** Utilize clear acrylic for visibility and ease of monitoring, with precision cuts made by a laser cutter.
- **Assembly:** Detailed design using CAD software for optimal airflow and light distribution, followed by assembly of cut acrylic panels.

### Stage 2: Full-Size Incubator / Plant Grower

- **Scaling Up:** Refine the design based on lessons learned from the miniature prototype, using clear acrylic material for the full-size version.
- **Environmental Control Systems:** Integration of heating pads and temperature sensors for even heat distribution and accurate temperature monitoring.

### Stage 3: AI Integration for Automated Environmental Control

- **Electronics and Sensors:** Installation of temperature sensors, heating pads, cameras, NPK sensors and IR sensors for comprehensive monitoring and control.
- **AI System Development:** Collection of data on growth conditions for the development of an AI model to automatically adjust environment parameters.

## Inspiration

Inspired by similar projects and products, the journey began with designing the incubator, experimenting with different tools and materials, and gradually integrating electronics for temperature control.

![Incubator inspiration]({{site.baseurl}}/images/Incubator-inspiration.jpg)

## Implementation and Testing

- **Prototype Testing:** Each version of the incubator is thoroughly tested, from the miniature model to the full-scale AI-integrated system.
- **Calibration and Safety Measures:** Ensuring the accuracy, reliability, and safety of the incubator system.

By methodically following this roadmap, the project aims to leverage modern technology for creating optimal growth conditions for mushrooms, showcasing the power of DIY and technological innovation.

Box specs:
Should be made of clear acrylic which we can cut with the laser cutter. Should be 1.4m in height, 0.6m in width and 0.6m in length. 

Size of electronic components:

![datasheet for temp sensor.jpg]({{site.baseurl}}/images/datasheet-for-temp-sensor.jpg){: width="250" }

<br>

# Temperature sensor:
- Length: 48.5mm
- Width: 40mm
- Height: 15.15mm

# Heating pads:
- Length: 200mm
- Width: 60mm
- Power: USB

## Roadmap

### Stage 1: Miniature Mushroom Incubator Design and Assembly

#### Materials and Components
- **Acrylic Sheets:** Utilize clear acrylic for visibility and easy monitoring. Your dimensions suggest a significant size, but start with a scaled-down model if this is the initial prototype.
- **Laser Cutter:** Employ the laser cutter for precise cuts and etchings on the acrylic, ensuring perfect fit and assembly.

#### Assembly
- **Design:** Create a detailed design of the incubator using CAD software, considering the internal layout for optimal airflow and light distribution.
- **Cutting:** Use the laser cutter to cut the acrylic panels based on your design. Include slots for easy assembly and areas for inserting the electronic components.
- **Assembly:** Assemble the cut panels using acrylic glue or screws designed for acrylic, ensuring stability and airtightness where necessary.

### Stage 2: Full-Size Incubator / Plant Grower

#### Scaling Up
- Take lessons learned from the miniature prototype to refine the design.
- Maintain the clear acrylic material for the full-size version, ensuring that the larger panels are supported adequately to prevent bending or breaking.

#### Environmental Control Systems
- Integrate the heating pads and temperature sensors, ensuring even distribution of heat and accurate temperature monitoring throughout the incubator.

### Stage 3: AI Integration for Automated Environmental Control

#### Electronics and Sensors
- **Temperature Sensors:** Install these for precise climate control, considering the size and placement for accurate readings.
- **Heating Pads:** Strategically place the heating pads to provide uniform warmth, powered via USB for easy adjustments and power management.
- **Cameras and IR Sensors:** These will monitor the growth progress and detect any abnormalities in the mushrooms.
- **pH Sensors:** Essential for maintaining the substrate at optimal pH levels for mushroom growth.

#### AI System Development
- **Data Collection:** Use the sensors and cameras to collect data on growth conditions and mushroom health.
- **AI Model:** Develop or adapt an AI model capable of analyzing the collected data to adjust temperature, lighting, and pH levels automatically. This could involve machine learning algorithms trained on optimal growth conditions for various mushroom species.
- **Interface:** Design a user interface for monitoring and manual overrides, ensuring ease of use and accessibility for non-technical users.

#### Implementation and Testing
- **Prototype Testing:** Thoroughly test each version of the incubator, starting with the miniature model and progressing through to the full-scale AI-integrated system.
- **Calibration:** Calibrate sensors and the AI system using known standards and test runs to ensure accuracy and reliability.
- **Safety Measures:** Implement safety features, especially in the full-size model, to protect against overheating or other electrical hazards.

By following this roadmap, you can systematically develop a sophisticated mushroom incubator that leverages modern technology for optimal growth conditions. Your well-equipped workshops and clear planning position you excellently for success in this ambitious project.

## Progression

To start I looked for inspiration from similar projects and products online. Once I found one I liked (see inspiration) I started looking for options to make the vector graphic file for the cutout. At first I found VectorArt.AI which did not work as intended to form the cutout for my box (see vectai.jpg). 

Then I started searching for open libraries similar to Thingiverse but for vector graphics and laser cut projects and found [3axis.co](https://3axis.co/download/qommv2ro) (box cutout for 12mm plywood which needed to be adjusted for 6mm). 

I then set up my Inkscape to work with .eps files by following these instructions. In the end, this step was unnecessary as the file I got from 3axis.co was a .cdr which opened fine in Inkscape.

I then adjusted the design a bit, scaled to my desired dimensions, and exported the .svg file to the USB stick. I then went to the laser cutter and after setting everything up I noticed that I had to adjust the size of the cutout holes to fit the 3mm plywood.

After adjusting in Lightburn the laser cutting began and once it was finished I had cutouts for my incubator box. With some help from the team, we assembled the incubator box and I began thinking how to integrate my electronics (mainly the temperature controller and heating pads).
<br>
![Incubator box assembled]({{site.baseurl}}/images/box-assembled.jpg){: width="250" }

To do this I uploaded my progress including images of the box, electronics, and PDF manual for the electronics into a DIY GPT to figure out what challenges and possible solutions I could face.
<br>
![Uploading project parts to ChatGPT]({{site.baseurl}}/images/upload-project-parts-to-chatgpt.jpg){: width="250" }

Since the datasheet for the temperature controller was in Chinese I wanted to be extra safe and test out first with a bench power supply. Unfortunately I did not have access to one at the time so I constructed my own 12V power source using 2 9V batteries conencted in series to get 12V and converted the voltage to 12V with a buck converter.
<br>
![Testing with 2 9V batteries]({{site.baseurl}}/images/testing-with-2-9v-batteries.jpg){: width="250" }

Unfortunately I thought the controller was rated for 12V input, however it's operational voltage was 5V, which I realized only after accidentally destroying 3 temperature controllers.

After finally figuring out the 5V problem and understanding how the relay of the temperature controller works I wired everything up and the heating pads were finally heating up to the set temperature.

I then assembled the box and electronics to make sure everything works and fits together.

![Box assembled with working electronics]({{site.baseurl}}/images/Incubator-box-with-electronics-not-complete.jpg){: width="250" }

Satisfied with how everything fits together I started thinking of a more permanent fixture, however I did not want to use glue in case I would want to disassemble and reassemble the incubator later.

Since I did not have a lot of time as we were supposed to present the next day I decided to 3D print only 2 [triple corner joints](https://www.thingiverse.com/thing:38277) (to connect the backboard) and use 2 metal corner brackets that I found in the lab.
<br>
![3D printer triple corner joints]({{site.baseurl}}/images/3d-printed-triple-corner-joints.jpg){: width="250" }
![Box with corner joints]({{site.baseurl}}/images/box-with-joints.jpg){: width="250" }
