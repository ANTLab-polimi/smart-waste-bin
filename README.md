# Take the trash out... to the edge. Creating a Smart Waste Bin based on 5G Multi-access Edge Computing.
The fifth generation of mobile cellular networks (5G) will bring many improvements to our everyday lives. In particular, the interplay between 5G and IoT technologies will pave the way for the realisation of the Smart City concept, providing humans with better, safer and cleaner cities. In this work, we describe the prototype of a Smart Waste Bin, a connected trash bin that automatically sorts garbage with the help of Convolutional Neural Networks algorithms. The bin intelligence runs on the edge of the 5G network exploiting a Mobile Edge Computing (MEC) architecture, enabling a low-latency and energy efficient operation. We describe the design, the implementation and the experimental validation of the prototype, also discussing possible future application scenarios.

## Dataset
This repository gathers the pictures used for the Waste Classification Algorithm training of the Smart Waste Bin (SWB). 
Pictures are taken directly in the Waste Disposal Unit of the SWB and are intended to be used only on this particular device.

Since entirely different objects may belong to the same recycling class (e.g., a plastic bottle and a plastic fork belong to the same plastic category), we split the classification task into two steps: -
1. The image is classified into the object by the AI; 
2. The object is classified into material. 

For instance, an image of a glass bottle is first classified as a glass bottle, and then a conditional algorithm classifies the glass bottle as glass.

![waste pictures](https://github.com/ANTLab-polimi/smart-waste-bin/blob/main/waste.png?raw=true)
Figure: A sample of the pictures used as training dataset. The objects are photographed by the Image Acquisition Module directly on the white shelf of the Waste Disposal Unit.

### Classes
The Waste Classification Algorithm is trained for five trash classes: 
- Paper 
- Glass
- Plastic
- Aluminium
- Unsorted

- (Optional, empty area)

### Objects
- Glass
  + Coke
  + Beer Becks
  + Aperol Bottle
  + Heineken Beer Bottle
  + Jar
  + Red Beer
  + Water Bottle
  
- Paper
  + Business Card
  + Candy Box
  + Cup
  + Flyers
  + Paper Bag
  + Juice Box
  + Magazine
  + Paper Napkins
  + Newspaper

- Plastic
  + Blue Bottle
  + White Bottle
  + Green Bottle
  + Coffee Capsule Packet
  + Transparent Glass
  + White Dish
  + Green Dish
  + Red Dish
  + Cutlery
  + Estathè bottle
  + Fiesta Packet
  + Yogurt Cup
  + Bag

- Aluminium
  + Coke Can
  + Fanta Can
  + Sprite Can
  + Redbull Can
  + Box
  + Coke Zero Can
  + Foil
  + Estathè Can
  + Jar Lid

- Unsorted
  + Backing Paper
  + Bic Pen
  + Pen
  + CD
  + Cigarettes
  + Lighter
  + Marker
  + Receipt
