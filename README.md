#  2.5V Precision Reference

A compact 2.5V precision voltage reference module, ideal for use as a standalone reference when building analog circuit prototypes or for verifying the accuracy of your multimeter’s voltage range over time.


## PCB Layout

![PCB](Photos/REF03_Kicad_PCB_Layer.png)

## Renders

![Render 1](Photos/REF03_Render.png)


![Render 2](Photos/REF03_Render2.png)

---
## Dimensions
![Dimensions](Photos/REF03_Dimensions.png)


## Features

- Single Coin Cell Operation
- TRIM pot for fine adjustment of output voltage
- 4mm BNC Terminal with 3/4" spcaing
- Compact Design with M2 mounting holes. 

---

## Datasheet
Datasheet: [Precision 2.5 V, 5.0 V, and 10.0 V
Voltage References](https://www.analog.com/media/en/technical-documentation/data-sheets/ref01_02_03.pdf)

```plaintext
## Some Design Afterthought's

The datasheet states the minimum operating of the REF03 should be 4.5V but during testing the output voltage remained stable upto 3V with no Load.
If the application has a requirement to sink some current, the supply voltage should be well above the minimum limits. A cut-off voltage circuit should be implemented to make sure the supply voltage remains above the minimum operating voltage.


```
