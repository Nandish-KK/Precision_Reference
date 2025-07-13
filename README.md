#  2.5V Precision Reference

A compact 2.5V precision voltage reference module, ideal for use as a standalone reference when building analog circuit prototypes or for verifying the accuracy of your multimeter’s voltage range over time.


## Prototyping and Testing
In order to make the Reference module compact the main requirement was to use lower voltage. A CR2032 coin cell at 3V is the ideal candidate.
This requirement turns into a design constrain as the minimum operating votage stated in the datasheet for the REF03 is 4.5V. The REF03 is a Low-Dropout
type Reference and is the best option to design a voltage reference due to its extremly low Temprature coefficient (10-50 ppm/C) and requires minimum passive
to operate.

In order to generate a voltage that is sufficient to drive the REF03 above the minimum operating voltage a charge pump topology is implemented.
The charge pump consist of a variable frequency oscillator and a voltage doubler circuit. The oscillator is constructed using SN74 logic inverter with
hystersis and a RC feedback network. At 3V input the circuit can generate a maximum of 5.6V but drops drastically depending on the load.
The quiescent current of the REF03 is around 1 ma which also gives a bit of headroom to even sink some current into the DUT. 


## PCB Layout
![PCB](Photos/REF03_Kicad_PCB_Layer.png)

## Renders

![Render 1](Photos/REF03_Render.png)


![Render 2](Photos/REF03_Render2.png)

---
## Dimensions
![Dimensions](Photos/REF03_Dimensions.png)

- PCB Diameter : 45mm
- Binding Post spacing : 19.05mm 
- Mounting Holes : 2.2mm





## Features

- Single Coin Cell Operation (CR2032).
- TRIM pot for fine adjustment of output voltage.
- 4mm BNC Terminal with 3/4" spacing.
- Adjustment Range 2.3V - 2.8V.
- Compact Design with M2 mounting holes and Toggle switch.

---

## Datasheet
Datasheet: [Precision 2.5 V, 5.0 V, and 10.0 V
Voltage References](https://www.analog.com/media/en/technical-documentation/data-sheets/ref01_02_03.pdf)

```plaintext
## Some Design Afterthought's

## 💡 Design Notes

- The REF03 datasheet specifies a minimum operating voltage of 4.5 V.
- However, during testing, the output remained stable down to 3 V with no load.
- If your application sinks significant current, ensure supply voltage remains well above the minimum — ideally with a low-voltage cutoff circuit.
- Also the toggle switch seems to be upside down.. D'oh!



```
