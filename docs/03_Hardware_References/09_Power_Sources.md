# Input
You can power up the board in 2 ways:

* **19V DC Power Jack** min 3.15A (60W) for basic functionalities.
* 2x **USB Type-C** power in. PD sink profile 20V/3A(60W).

A bicolour Green/Yellow LED is placed near the DC IN power jack (CN5) to signal the power state of the board.  
When the board is powered but turned off, then the LED turns on Yellow, during normal working (S0 State) the LED turns on Green light.

## DC Power Jack
The UDOO BOLT board can be supplied with an external **19VDC ± 5%** power supply, minimum **60W** (i.e. min. *3.15A @ 19V*) for basic functionalities recommended.

<span class="label label-warning">Heads up!</span> Always make sure that the power cable is less than *3mt.* long.

This voltage can be supplied through a DC power jack (CN5).

**Mating DC** plug is a male connector **4.5mm x 3.0mm with pin inside**.

<span class="label label-warning">Heads up!</span> CE and FCC certifications retained using only the UDOO BOLT qualified Power Supply you can find in the UDOO Shop. When not using UDOO Gear qualified Power Supply, use 19VDC (min 60W power) PSUs certified for your country

## USB Type-C

The Board can also be powered by using a standard **USB-C** power adapter thanks the **Power Delivery** in **Sink mode**.  
You can use either one of the two USB Type-C connectors *(CN8, CN9)*.  
The **PD Sink** power profile is **20V 3A**.

<br>

<span class="label label-info">Info</span> In this thread of the UDOO Forum you can find an *unofficial* (but really useful) discussion about others compatible power supplies: [Power supply compatibility list](https://www.udoo.org/forum/threads/power-supply-compatibility-list.27218/)

# Output

## USB Type-C

In **Power Delivery Source Mode** (in output from the Gear to a USB device) the output is **5V 3A** *max* per port with an overall budget of **4A**, ie if a device connected to one port is consuming 3A, the other port has maximum 1 other Ampere to be given in output.

## USB 3.0 Type A

The output from a USB 3.0 Type A to a USB device is the standard for USB3 specs, up to 900mA (0.9A).
