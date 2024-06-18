Raspberry Pi Pico pinout diagram

                              ┌╌ LED (GP25)
                              ┆ ┏━━━━┓
                          ┌─────┃    ┃─────┐
    | SPI0 RX  | GP0  | 01│●  ┆ ┗━━━━┛    ●│40 | VBUS
    | SPI0 CSn | GP1  | 02│●  ⏄           ●│39 | VSYS
                 GND  | 03│■              ■│38 | GND
    | SPI0 SCK | GP2  | 04│●    ╭─╮       ●│37 | 3V3_EN
    | SPI0 TX  | GP3  | 05│●    │ │       ●│36 | 3V3(OUT)
    | SPI0 RX  | GP4  | 06│●    ╰─╯       ●│35 |
    | SPI0 CSn | GP5  | 07│●              ●│34 | GP28
                 GND  | 08│■              ■│33 | GND
    | SPI0 SCK | GP6  | 09│●   ┌─────┐    ●│32 | GP27
    | SPI0 TX  | GP7  | 10│●   │     │    ●│31 | GP26
    | SPI1 RX  | GP8  | 11│●   │     │    ●│30 | RUN
    | SPI1 CSn | GP9  | 12│●   └─────┘    ●│29 | GP22
                 GND  | 13│■              ■│28 | GND
    | SPI1 SCK | GP10 | 14│●              ●│27 | GP21     |
    | SPI1 TX  | GP11 | 15│●              ●│26 | GP20     |
    | SPI1 RX  | GP12 | 16│●              ●│25 | GP19     | SPI0 TX
    | SPI1 CSn | GP13 | 17│●              ●│24 | GP18     | SPI0 SCK
                 GND  | 18│■              ■│23 | GND
    | SPI1 SCK | GP14 | 19│●              ●│22 | GP17     | SPI0 CSn
    | SPI1 TX  | GP15 | 20│●     ● ■ ●    ●│21 | GP16     | SPI0 RX
                          └────────────────┘
                                 ┆ ┆ ┆
                                 ┆ ┆ └╌ SWDIO
                                 ┆ └╌╌╌ GND
                                 └╌╌╌╌╌ SWCLK

Display Pinout:

    Port Number	| Port Name	    |    Mapping
    1	        | BUSY	        |    Status Indication
    2	        | RES	        |    Reset
    3	        | D/C	        |    Data/Command
    4	        | CS	        |    Chip Select (CS)
    5	        | SCL	        |    Serial Clock (SCLK)
    6	        | SDA	        |    Serial Data (MOSI)
    7	        | GND	        |    Ground (GND)
    8	        | VCC (3.3V)	|    Power Supply (3.3V)

Connections:

    Display Port	Display Port Name	Pico Pin	Pico Pin Function
    1	                BUSY	            -	           - (not connected, status indication)
    2	                RES	                GP17	        GPIO (can be used as a general purpose pin)
    3	                D/C	                GP16	        GPIO (Data/Command control)
    4	                CS	                GP5	            SPI0 CSn (Chip Select)
    5	                SCL	                GP18	        SPI0 SCK (Serial Clock)
    6	                SDA	                GP19	        SPI0 TX (Serial Data MOSI)
    7	                GND	                GND	            Ground (any GND pin)
    8	                VCC (3.3V)	        3V3(OUT)	    Power Supply (3.3V)
