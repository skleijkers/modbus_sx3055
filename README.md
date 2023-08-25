# Home Assistant modbus configuration for Solarfam SX3055

Home Assistant modbus configuration for a serial (RS485) attached Solarfam SX3055. Tested with a Waveshare USB to RS485 stick (https://www.waveshare.com/usb-to-rs485.htm).

This configuration has been made for the Solarfam SX3055, but it's expected that this configuration will also work for the following MPPT Charge Controllers of SolarFam and Lumiax:
- SolarFam SX2010 (MT2010)
- SolarFam SX3055 (MT3010)
- Lumiax MT2010
- Lumiax MT2075
- Lumiax MT3075
- Lumiax MT3010
- Lumiax MT4010
- Lumiax MT4015

In fact the two SolarFam MPPT Controller are relabeled Lumiax MPPT Controllers.

# Install

Open terminal in Home Assistant

cd config

git clone https://github.com/skleijkers/modbus_sx3055 sx3055

Add the following lines to configuration.yaml:

modbus: !include sx3055/sx3055.yaml

template: !include sx3055/sx3055_template.yaml

