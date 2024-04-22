# Building the Glove

This is a building instruction for the glove needed to build the the [Unfolding Space Glove](https://github.com/jakobkilian/unfolding-space).

## Overview

The glove has two layers of fabric with the vibration motors and cables in between. There is velcro to attach the Unfolding Space Carrier Board (see pcb directory of this repo) to it and a ribbon cable exiting the back of the glove terminating with an idc connector to link glove and board. The end result looks like this (two sizes: red = big and purple = small): 

![The glove when it is finished. There are two sizes: red = big and purple = small](images/glove-overview.jpg)

## 1. Textile Work

First of all, we need the inner and outer layers of the glove. You could sew these yourself, but this is very time-consuming. I therefore looked for suitable models which I could work with. It quickly became clear that both gloves had to be very thin, because otherwise the construction would be too thick and uncomfortable. In order to achieve a high degree of stretch and durability at the same time, I looked primarily for polyamide textiles. Most of them are work gloves with coating, which made the search more difficult.

I found what I was looking for in a very thin inner layer of a polyamide [clean room glove ](https://www.munitec-gmbh.de/polyamid-reinraum-handschuhe-glatt.html)(article number 12025) from Munitec (they were kind enough to provide me with samples of their collection). They can also be cut well without becoming frayed.

The outer layer should meet basic aesthetic requirements, look neutral and also be stretchable and resistant. Here it was a no name (Worksafe L71-720) product from Amazon (though I hate buying there).

### Outer Layer

I cut the fingers of the gloves halfway so that the two sizes would fit as well as possible on different hands. 

| Cut the Fingers Halfway                                                                                              |
|:--------------------------------------------------------------------------------------------------------------------:|
| ![A kitchen knife next to the cut-in-half finger of the black glove on a wooden surface.](images/_DSC0007mod_lq.jpg) |
| To avoid fraying in the first place, it proved most effective to use a sharp kitchen knife                           |

Since I don't have a tool to hem the cut edges of the fingers (no idea how that would work), I experimented a bit with anti-fraying glue and the like and finally settled on liquid latex, typically used to make anti-slip socks. With some wooden stuffing of the fingers I was able to dip them into the latex and cut a clean edge after drying:

| Stuffing Material                                                                       | Just Before Dipping                                                                                                 |
|:---------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------:|
| ![Short pieces of a wooden stick used as stuffing material.](images/_DSC0003mod_lq.jpg) | ![The fingers of the glove stuffed with the pieces of wooden stick just before dipping.](images/_DSC0008mod_lq.jpg) |

| After Dipping                                                                                           | Drying...                                                                          |
|:-------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------:|
| ![Fresh, grey liquid latex at the fingertips of the glove after dipping it.](images/_DSC0011mod_lq.jpg) | ![Suspended glove with drying latex on the fingertips.](images/_DSC0032mod_lq.jpg) |

| Getting Rid of Overhang                                                       | Finish Edges                                                                                                                |
|:-----------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------:|
| ![A cutter cuts away the overhanging latex lumps.](images/_DSC0089mod_lq.jpg) | ![A small pair of scissors lies on the table next to the glove. Fine cuttings lie next to them.](images/_DSC0092mod_lq.jpg) |

Resulting in these edges that do their job of not fraying and not looking too bad:

| Result                                                                                                         |
|:--------------------------------------------------------------------------------------------------------------:|
| ![Macro shot of several gloves with focus on the finished, hemmed fingertips](images/_DSC0199mod_lq-edges.jpg) |

## Inner Layer

Next I determined the position of the motors so that they are equally spread over the available surface and do not interfere with hand movements. 

| Positioning of the Motors                                                                                                                             | Reproducing Inner Layers                                                                                            |
|:-----------------------------------------------------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------:|
| ![A sliding gauge and the thin, white, inner glove layer on which points can be seen where the motors are to be attached.](images/_DSC0040mod_lq.jpg) | ![Two of the inner layer gloves with the same markings for motors, board and the like. ](images/_DSC0073mod_lq.jpg) |

The inner gloves were cut in the same way as the outer ones but with slightly longer fingers so that they could be folded over and sewn by hand to the outer glove (no picture).

## 2. Preparing the Motors and Cables

Regarding the motors experience from older prototypes revealed two particular weaknesses that can occur when there is a lot of physical stress: 

- The **breaking of the solder joints** on the vibration motor's solder pad.
- The **tearing of cables from the connector** on the other side due to excessive tensile stress. These occur due to the great mobility of the hands.

To prevent **breaking of the solder joints**, I soldered the cables onto the soldering pad so that they ran past the motor to the rear. If you then wrap the entire motor in a heat-shrink tube, the soldering point is relieved of strain in a cost-effective way and the problem is solved. 

| Soldering of the cables                                                                          |
|:------------------------------------------------------------------------------------------------:|
| ![An affixed vibration motor which just gets a lead end soldered on.](images/_DSC0063mod_lq.jpg) |

| Add Heat Shrink Tubing                                                                                                                        | Shrink Them                                                                               |
|:---------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| ![A heat shrink tubing around three motors, the cables coming out of them on the opposite side of the solder pad.](images/_DSC0065mod_lq.jpg) | ![The tubing shrunk tightly around the motors and the cables.](images/_DSC0070mod_lq.jpg) |

| Before and After                                                                                        |
|:-------------------------------------------------------------------------------------------------------:|
| ![A bare motor without cables and the soldered, and shrunk version besides.](images/_DSC0027mod_lq.jpg) |

Next to prevent **tearing of cables from the connector** I tried to route the cables in a meandering way on the inner layer of the glove so that they bypass all the joints of the hand that can cause tension on the cable.

| Routing Experiments                                                                                                                  |
|:------------------------------------------------------------------------------------------------------------------------------------:|
| ![The thin, white, inner textile layer with short cables taped on it to demonstrate a possible routing](images/_DSC0054mod_lq.jpg)   |
| With this routing, the cable is not heavily stressed by any the movement of the hand. The dots represent the position of the motors. |

| Testing the Cable Exit Point                                                                                                                         |
|:----------------------------------------------------------------------------------------------------------------------------------------------------:|
| ![A flat ribbon cable exiting the outer, black layer of the glove at its back through a cutted slot to test the routing.](images/_DSC0106mod_lq.jpg) |
| Testing the exit point of the flat ribbon cable that is used in the final setup.                                                                     |

## 3. Implementation of the Wiring

With the routing being determined, I could produce the wiring strands using flat ribbon cables:

| Cutting, Soldering, Wrapping                                                                                          | Apply Adhesives to Motors                                                                                |
|:---------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------:|
| ![A flat ribbon cable with the motors soldered to the wires placed on a ruler.](images/IMG_20210710_163652mod_lq.jpg) | ![The finished motors in shrink tubing with adhesive surfaces on the bottom.](images/_DSC0148mod_lq.jpg) |

| Crimping the IDC Connector & Testing Connections                                                |
|:-----------------------------------------------------------------------------------------------:|
| ![A multimeter that measures individual pins of the IDC connector..](images/_DSC0141mod_lq.jpg) |

| Resulting Wiring Glued onto the Glove                                                           |
|:-----------------------------------------------------------------------------------------------:|
| ![A multimeter that measures individual pins of the IDC connector..](images/_DSC0111mod_lq.jpg) |

## 4. Sewing of the Cables

The cables then had to be sewed onto the glove by hand. For this I used a cardboard hand from the craft shop that. 

| Sewing                                                                                                                                   |
|:----------------------------------------------------------------------------------------------------------------------------------------:|
| ![The glove affixed on the carboard hand and in bright lighting condition gets sewed with needle and thread.](images/_DSC0185mod_lq.jpg) |
| The quite time consuming process of sewing all cables onto the inner textile layer                                                       |

| Result                                                                                                                       |
|:----------------------------------------------------------------------------------------------------------------------------:|
| ![Close up of the glove affixed on the carboard hand. Now with finished seams fixing the cables.](images/_DSC0161mod_lq.jpg) |
| ![Close up of a seam around a cable only](images/IMG_20210716_154432mod_lq.jpg)                                              |

Now the already joined outer part of the glove could be put over the inner part and the glove was practically completed.

| Steps of Implementation                                                                                                                                                                                                                                                                                                                                                    |
|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| ![Three steps of implementation: First, the wiring, the inner and the outer glove layer spearated on the table. Second, these three components got sewed together. The wiring onto the inner glove and the fingers of the inner with the outer layer. Third shows the completed glove with the outer layer put over the inner.](images/IMG_20210717_145153mod_numbers.jpg) |
| 1) The three components separated. 2) Sewing of components completed. 3) Glove completed                                                                                                                                                                                                                                                                                   |

## 5. Adding Velcros and Finishing

Finally, I added some Velcro: firstly, to attach the "Unfolding Space Carrier Board" to the glove; secondly, to connect the inner and outer layers at the wrist without sewing them together, so that you can open them in case of error.

| Sewing the Velcros                                                                        |
|:-----------------------------------------------------------------------------------------:|
| ![A sewing machine with someone sewing Velcro onto the glove.](images/_DSC0186mod_lq.jpg) |
| The sewing of the velcros was done with a sewing machine.                                 |

| Velcros for the Carrier Board                                                                                                                                                 |
|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
| ![You can see the Velcro fasteners on the back of the glove and the Unfolding Space Carrier Board, which also has Velcros and folds away upwards.](images/_DSC0133mod_lq.jpg) |
| The velcros for fastening the carrier board and the slot where the ribbon cable exits the glove.                                                                              |

## Result

 ![The glove on a table. Tools, a ruler, a scissor and the carrier board besides. The glove is now finished with velcros attached. ](images/_DSC0135mod_lq.jpg)

 ![Four finished glove models next to each other. ](images/_DSC0199mod_lq.jpg)

**If you have any questions, feel free to mail me!**
