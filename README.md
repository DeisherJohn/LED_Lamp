

# LED Lamp ReadMe <!-- omit in toc --> 
Included below is information about a homemade LED lamp with different control features for home use. The idea of this project is to create a LED desklamp that has knobs. The knobs will change the colors and brightness of the lamp. The final design will take into account kids ages ~5+ to using it unsupervised.

# Table of Contents  <!-- omit in toc -->
- [1. Overview](#1-overview)
  - [1.1. The Idea](#11-the-idea)
  - [1.2. Parts Overview](#12-parts-overview)
- [2. Requirements](#2-requirements)
  - [2.1. Power](#21-power)

# 1. Overview

This section will include a general overview of the project. 

## 1.1. The Idea

This idea came about thinking about a gift for my niece. We have put together different toys in the past, and she seemed to have fun dealing with small things that we could put together. I wanted to create a lamp with installable parts we could build together for her to use. This project needed to be something that she would use for a few years at least, and any components that are likely to give out should be relatively easy to replace. Using this, I decided to include physical knobs that she can use to adjust and mix the color to her liking. This choice was two-fold.

- First: it allows her to match the lamp colors to her mood or room as she sees fit, increasing the useful lifespan of the lamp. 
- Second: this will teach her color theory as she will be mixing the colors using RGB knobs instead of a color pallet. 

While working on the design, I decided to add greater user control through an app. This choice means that any microcontroller selected will need to support Bluetooth communications. 

## 1.2. Parts Overview

---

### **Microcontroller:**<!-- omit in toc --> 

---

I have used Teensy Microcontroller in the past, and they have performed well in every project. As I wanted items that would be easy and relatively cheap to use, I selected the Teensy LC as my microcontroller. 

Benefits: 
- Multiply Analog ports
- Several digital IO ports
- Vast software libraries (for both LEDs and Bluetooth)
- Easy of use for prototyping

### **LED Strip:**<!-- omit in toc --> 

---

With the inclusion of Bluetooth in this project, I opted for more control of the LEDs by using addressable LED strips. Since this is a basic prototype, it will focus on the WS2812B addressable LED strip. If possible, the final design will come with connectors for both the WS2812B and the WS2813 allowing for a broader range of compatible LED strips. 
    
**WS2812B:** 

This LED strip has fully addressable LEDs, is low-cost for addressable LEDs, and is widely supported by many LED libraries. The WS2812B uses a three-pin JST connector. 

**WS2813:** 

The WS2813 LED strip cost more than the WS2812B but a backup data line so that if one LED burns out, the other LEDs on the strip will continue to function. The WS2813 should be used when lifespan is more important than cost. The WS2813 uses a four-pin JST connector. 

### **Knobs:**<!-- omit in toc --> 

---

For this project, I will be using 10k Ohm 1-turn potentiometers as the color and brightness knobs. 

# 2. Requirements

Listed below are different requirements this project will meet or attempt or attempt to meet as specified by each item. 

## 2.1. Power 

---

Below are all the requirements for this project relating to power. 

### Input Power <!-- omit in toc --> 

    Acceptable Input Voltage Range: 110-240V @ 50-60Hz.

### Output Power <!-- omit in toc --> 

    Part of this design will include an option outlet should an end-user wish to use it. In this case, the output plug voltage will follow the input voltage requirements. 



