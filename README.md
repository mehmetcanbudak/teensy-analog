# teensy-analog
Notes and ideas about how to interface teensy mcu with analog in/out

*( * DAS - data-acquisition system)*

# audio-class 
# control-voltage class
## ADC
* [Analog Devices precision dac](https://www.analog.com/en/products/digital-to-analog-converters/standard-dac/precision-dac/bipolar-da-converters.html)
  * [AD7606](https://www.analog.com/en/products/ad7606-6.html) 
    * 8-/6-/4-Channel DAS with 16-Bit, Bipolar Input, Simultaneous Sampling ADC  
    * analog input ranges: ±10 V, ±5 V
    * Single 5 V analog supply and 2.3 V to 5 V VDRIVE
    * [datasheet](https://www.analog.com/media/en/technical-documentation/data-sheets/ad7606_7606-6_7606-4.pdf)
  * [AD7608](https://www.analog.com/en/products/ad7608.html)
    * 8-Channel DAS with 18-Bit, Bipolar, Simultaneous Sampling ADC
    * [datasheet](https://www.analog.com/en/products/ad7608.html)
## DAC
* [AD5362](https://www.analog.com/en/products/ad5362.html)
  * 8-Channel, 16-Bit, Serial Input, Voltage-Output DAC
  * output voltage range of -10 V to +10 V
  
## DAS
* MAX11300
  * 20-Port Programmable Mixed-Signal I/O with 12-Bit ADC, 12-Bit DAC, Analog Switches, and GPIO  
  * SPI bus
  * [datasheet](https://www.maximintegrated.com/en/products/analog/data-converters/analog-to-digital-converters/MAX11300.html)
