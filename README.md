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

# analog devices DAC candidates
  * [bipolar-da-converters](https://www.analog.com/en/products/digital-to-analog-converters/standard-dac/precision-dac/bipolar-da-converters.html)

|Part#|# of Channels|Resolution(bits)|Interface|Vout Range|DAC INL(max)(LSBs)|Settling Time(typ)(s p-p)|Power(typ)(W)|Price (1000+)($ US)|
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
|AD5766|16|16|SPI|±10V, ±5V, -10to0V, -10to6V, -12to14V, -16to0V, -16to10V, -20to0V|16|16µ|-|$35.00 (AD5766BCBZ-RL7)|
|LTC2664-16|4|16|SPI|±10V, ±2.5V, ±5V, 0to10V, 0to5V|4|9µ|21m|$15.60 (LTC2664CUH-16#PBF)|
|LTC2666-16|8|16|SPI|±10V, ±2.5V, ±5V, 0to10V, 0to5V|4|4.5µ|37m|$21.75 (LTC2666CUH-16#PBF)|
|LTC2668-16|16|16|SPI|±10V, ±2.5V, ±5V, 0to10V, 0o5V|4|9µ|73m|$31.25 (LTC2668CUJ-16#PBF)|
|LTC2754B-16|4|16|SPI|±10V, ±2.5V, ±5V, 0to10V, 0to5V, -2.5Vto7.5V|1|2µ|1.5µ|$17.85 (LTC2754BCUKG-16#PBF)|
|LTC2754A-16|4|16|SPI|±10V, ±2.5V, ±5V, 0to10V, 0to5V, -2.5Vto7.5V|1|2µ|1.5µ|$19.70 (LTC2754ACUKG-16#PBF)|
|AD5754R|4|16|SPI|±10V, ±10.8V, ±12V, ±5V, 0to10V, 0to10.8V, 0to5V|16|7.5µ|310m|$13.34 (AD5754RBREZ)|
|AD5752R|2|16|SPI|±10V, ±10.8V, ±12V, ±5V, 0to10V 0to10.8V, 0to5V|16|7.5µ|190m|$9.22 (AD5752RBREZ)|
|AD5764R|4|16|SPI|±10.5V, ±14V|1|8µ|275m|$28.35 (AD5764RBSUZ)|
|AD5754|4|16|SPI|±10V, ±10.8V, ±12V, ±5V, 0to10V, 0to10.8V, 0to5V|16|7.5µ|310m|$10.35 (AD5754AREZ)|
|LTC2704-16|4|16|SPI|±10V, ±2.5V, ±5V, 0to10V, 0to5V, -2.5Vto7.5V|2|4µ|172.5m|$29.95 (LTC2704CGW-16#PBF)|
|AD5764|4|16|SPI|±10.5V, ±14V|1|8µ|381m|$23.33 (AD5764ASUZ)|
|AD5734R|4|14|SPI|±10V, ±10.8V, ±12V, ±5V, 0to10V, 0to10.8V, 0to5V|4|7.5µ|310m|$11.28 (AD5734RBREZ)|
|AD5732R|2|14|SPI|±10V, ±10.8V, ±12V, ±5V, 0to10V, 0to10.8V, 0to5V|4|7.5µ|190m|$7.73 (AD5732RBREZ)|
|AD5744R|4|14|SPI|±10.5263V, ±14.7368V|1|8µ|387m|$24.31 (AD5744RCSUZ)|
|AD5732|2|14|SPI|±10V, ±10.8V, ±12V, ±5V, 0to10V, 0to10.8V, 0to5V|4|7.5µ|190m|$5.67 (AD5732AREZ)|
|AD5734|4|14|SPI|±10V, ±10.8V, ±12V, ±5V, 0to10V, 0to10.8V, 0to5V|4|7.5µ|310m|$8.50 (AD5734AREZ)|
|LTC2704-14|4|14|SPI|±10V, ±2.5V, ±5V, 0to10V, 0to5V, -2.5Vto7.5V|1|3.5µ|172.5m|$24.95 (LTC2704CGW-14#PBF)
