# VCC GND STM32F407ZGT6 Mini

MicroPython board definition files for the STM32F407ZGT6 Mini board from [VCC-GND](http://vcc-gnd.taobao.com).

![board](docs/STM32F407ZGT6.jpg)

You can buy one for around $17 AUD on [Taobao](https://item.taobao.com/item.htm?id=523383164199).

Clone the board definitions to your [MicroPython](https://github.com/micropython/micropython) `ports/stm32/boards` folder.

```
cd micropython/ports/stm32/boards
git clone https://github.com/mcauser/VCC_GND_F407ZG.git
```

### Build the firmware:

```
cd micropython/ports/stm32
make BOARD=VCC_GND_F407ZG
```

### Exposed Port Pins

* PA0-PA15
* PB0-PB15
* PC0-PC15
* PD0-PD15
* PE0-PE15
* PF0-PF15
* PG0-PG15

### Specifications:

* STM32F407ZGT6 ARM Cortex M4
* 168MHz, 210 DMIPS / 1.25 DMIPS / MHz
* 1.8V - 3.6V operating voltage
* 25MHz system crystal (NX5032GA)
* 32.768KHz RTC crystal
* AT24C08 I2C EEPROM 1024 Byte x 8, 400KHz
* W25X40BVSNIG SPI Flash 4Mbit (512x8bit), 104 MHz
* 2.54mm pitch pins
* JTAG/SWD header
* 1024 KByte Flash, 192 + 4 KByte SRAM
* 3x SPI, 3x USART, 2x UART, 2x I2S, 3x I2C
* 1x FSMC, 1x SDIO, 2x CAN
* 1x USB 2.0 FS / HS controller (with dedicated DMA)
* 1x USB HS ULPI (for external USB HS PHY)
* Micro SD
* 1x 10/100 Ethernet MAC
* 1x 8 to 12-bit Parallel Camera interface
* 3x ADC (12-bit / 16-channel)
* 2x DAC (12-bit)
* 12x general timers, 2x advanced timers
* RT9193-3.3V: 3.3V LDO voltage regulator, max current 300mA
* Micro USB for power and comms
* User LED (PG15)
* 2x DIP switch for bootloader selection
* Reset button
* 2x22 side pins + 2x6 top pins + 2x13 bottom pins, 1x4 J-Link pins
* Dimensions: 59.69mm x 46.99mm

### Modifications:

* change HSE_VALUE from 8000000 to 25000000
* change PLL_M from 8 to 25

### Links:

* [STM32F407ZG on st.com](https://www.st.com/en/microcontrollers-microprocessors/stm32f407zg.html)
* [Buy on AliExpress](https://www.aliexpress.com/item/STM32F407ZGT6-Mini-Version-of-the-Core-Board-Minimum-System-Version-STM32/32819158767.html) or search for "STM32F407ZGT6 Mini"
* [Buy on Taobao](https://item.taobao.com/item.htm?id=523383164199)
* [STM32F407 datasheet](docs/STM32F407_datasheet.pdf)
* [STM32F407ZGT6 mini schematics](docs/STM32F407ZGT6_schematics.pdf)
* [STM32F407ZGT6 mini PCB](docs/STM32F407ZGT6_mini.pdf)
* [STM32F4 alternate function mapping](docs/STM32F4-AF-mapping.pdf)
* [Smaller STM32F407VET6 mini board](https://github.com/mcauser/VCC_GND_F407VE)

## License

Licensed under the [MIT License](http://opensource.org/licenses/MIT).
