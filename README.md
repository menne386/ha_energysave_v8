# Home-Assistant modbus config files for EnergySave V8 heatpumps 
Modbus configuration files to integrate an energysave v8 heatpump system into Home-Assistant

## What it does:
- Read most important sensors from your heatpump
- exposes ON/OFF switch
- exposes switch between 'heating with curve' and a fixed thermostat
- Exposes 3 climate entities (for controlling hot water, zone1 heating and zone1 cooling)

## What you need:
- TCP to modbus adapter such as [this](https://www.waveshare.com/wiki/RS485_TO_ETH_(B))
- Correct serial configuration: Baud Rate 19200, Databits 8, Parity: none, Stopbits: 1, Flow control: None
- Correct modbus settings on the waveshare: Protocol: Modbus TCP to RTU.
- Static IP adres for the adapter

## Installation:

- Create a 'packages' folder. [See home-assistant documentation](https://www.home-assistant.io/docs/configuration/packages/)
- upload 'heatpump.yaml' into your packages folder
- edit heatpump.yaml and set the IP adres of your tcp/to/modbus adapter.



