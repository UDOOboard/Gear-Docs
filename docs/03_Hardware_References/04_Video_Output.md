The Graphic controller of the **UDOO BOLT GEAR** is the integrated **AMD Radeon&trade; Vega Graphics**.  

* **AMD Radeon™ Vega 8 Graphics** - Up to 1100 MHz 8 execution units

The AMD Radeon&trade; Vega Graphics controller offers extremely high graphical performances, supporting also **High Dynamical range (HDR)** Imaging. **DirectX® 12**, **EGL 1.4**, **OpenCL 2.1**, **OpenGL® ES 1.1/ 2.x / 3.x (Halti)**, **OpenGL® Next (Vulkan®)**, **OpenGL® 4.6** are also supported by this GPU, which can also offer **H.265** *10-bit video decoding* and *8-bit encoding*.


### Video Output Connectors

The UDOO BOLT GEAR is able to drive 4x 4K independent displays, by using the 2x HDMI 2.0 and the 2x USB-C interfaces available.
The AMD Ryzen Embedded V1000 family of Processors offer four Digital Display Interfaces, configurable to work in HDMI/DVI/DP++ modes.

#### HDMI Connectors

On the UDOO BOLT GEAR board, the Digital Display Interfaces #0 and #1 are used to implement two **HDMI 2.0** interfaces through as many HDMI ReDriver / Level shifters and ESD protection + signal conditioning ICs.

Maximum resolution:
* 4096x2160 @ 60Hz

<span class="label label-warning">Heads up!</span>  Always use HDMI-certified cables for the connection between the board and the HDMI display; a category 2 (High-Speed) cable is recommended for higher resolutions, category 1 cables can be used for 720p resolution.

You can use this [HDMI to HDMI](http://shop.udoo.org/cable-hdmi-to-hdmi.html) cable to connect to a HDMI display in 4k resolution.

#### USB-C Connectors win DipslayPort Alternate Mode

USB 3.1 Port #0 is internally multiplexed by the AMD Ryzen Embedded V100 Processor with Display Port #3, USB 3.1 Port #3 is multiplexed with Display Port #2., i.e. its can be used to support USB-C Displays or DP displays directly and, through an external adapter, also HDMI or DVI displays.  
The configuration of this interface in DP or HDMI/DVI mode is automatic.

Maximum resolution:
* 4096x2160 @ 60Hz

In the market, you can find USB-C Touch Displays with a single USB-C cable to power the display, send the video signal and receive the touch signal.
In addition, there are displays that provide power via USB-C. Once the display is connected to a standard power supply, they allow the UDOO BOLT GEAR to be powered by a single USB-C cable and receive the video signal.
