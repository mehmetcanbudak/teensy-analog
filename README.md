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
    * QFP64 packaging
  * [AD7608](https://www.analog.com/en/products/ad7608.html)
    * 8-Channel DAS with 18-Bit, Bipolar, Simultaneous Sampling ADC
    * [datasheet](https://www.analog.com/en/products/ad7608.html)
## DAC
* [AD5362](https://www.analog.com/en/products/ad5362.html)
  * 8-Channel, 16-Bit, Serial Input, Voltage-Output DAC
  * output voltage range of -10 V to +10 V
* [AD5754R](https://www.analog.com/en/products/ad5754r.html)	AD5754BREZ
  * 4 channel 
  * 16-bit D/A converter
  * Operates from single/dual supplies
  * Software programmable output range
    * +5 V, +10 V, +10.8 V, ±5 V, ±10 V, ±10.8 V
  * [datasheet](https://www.analog.com/media/en/technical-documentation/data-sheets/ad5724r_5734r_5754r.pdf)
  * TSSOP24 (exposed pads) packaging

## DAS
* MAX11300
  * 20-Port Programmable Mixed-Signal I/O with 12-Bit ADC, 12-Bit DAC, Analog Switches, and GPIO  
  * SPI bus
  * [datasheet](https://www.maximintegrated.com/en/products/analog/data-converters/analog-to-digital-converters/MAX11300.html)


# connectors 
* vertical female connectors on [octopart](https://octopart.com/search?category_ids=5142&specs2.92.values=Female&start=0&specs2.20.values=Through%20Hole&specs2.523.values=Vertical)
* ACJS-MV35-5
* [3.5mm_jack_sockets on sdiy](https://sdiy.info/wiki/Eurorack_DIY_panel_components#3.5mm_jack_sockets)

# switching jacks
* [understanding-audio-jack-switches-and-schematics](https://www.cui.com/blog/understanding-audio-jack-switches-and-schematics)

# fixture testing
* [openfixture](https://github.com/tinylabs/openfixture)

# analog devices DAC candidates
  * [bipolar-da-converters](https://www.analog.com/en/products/digital-to-analog-converters/standard-dac/precision-dac/bipolar-da-converters.html)

|Part# |Channels|Resolution(bits)|Interface|Vout Range|Price|
|--- |--- |--- |--- |--- |--- |
| AD5362 | 8 |	16 |	SPI |	Vsupply Neg+1.4VtoVsupply-1.4V |$24.92 (AD5362BCPZ)|
|AD5766|16|16|SPI|±10V, ±5V, -10to0V, -10to6V, -12to14V, -16to0V, -16to10V, -20to0V|$35.00 (AD5766BCBZ-RL7)|
|LTC2664-16|4|16|SPI|±10V, ±2.5V, ±5V, 0to10V, 0to5V|$15.60 (LTC2664CUH-16#PBF)|
|LTC2666-16|8|16|SPI|±10V, ±2.5V, ±5V, 0to10V, 0to5V|$21.75 (LTC2666CUH-16#PBF)|
|LTC2668-16|16|16|SPI|±10V, ±2.5V, ±5V, 0to10V, 0o5V|$31.25 (LTC2668CUJ-16#PBF)|
|LTC2754B-16|4|16|SPI|±10V, ±2.5V, ±5V, 0to10V, 0to5V, -2.5to7.5V|$17.85 (LTC2754BCUKG-16#PBF)|
|LTC2754A-16|4|16|SPI|±10V, ±2.5V, ±5V, 0to10V, 0to5V, -2.5to7.5V|$19.70 (LTC2754ACUKG-16#PBF)|
|AD5754R|4|16|SPI|±10V, ±10.8V, ±12V, ±5V, 0to10V, 0to10.8V, 0to5V|$13.34 (AD5754RBREZ)|
|AD5752R|2|16|SPI|±10V, ±10.8V, ±12V, ±5V, 0to10V 0to10.8V, 0to5V|$9.22 (AD5752RBREZ)|
|AD5764R|4|16|SPI|±10.5V, ±14V|$28.35 (AD5764RBSUZ)|
|AD5754|4|16|SPI|±10V, ±10.8V, ±12V, ±5V, 0to10V, 0to10.8V, 0to5V|$10.35 (AD5754AREZ)|
|LTC2704-16|4|16|SPI|±10V, ±2.5V, ±5V, 0to10V, 0to5V, -2.5to7.5V|$29.95 (LTC2704CGW-16#PBF)|
|AD5764|4|16|SPI|±10.5V, ±14V|$23.33 (AD5764ASUZ)|
|AD5765|4|16|SPI|±4.096 V, ±4.201 V, ±4.311 V, ±4.421 V|$19.52 (AD5765CSUZ)|
|AD5544|4|16|SPI|-|$21.23 (AD5544ARSZ)|
