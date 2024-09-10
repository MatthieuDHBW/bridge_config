# Bridge configuration
This repo contains the configuration used with the [bridge](https://github.com/lkzjdnb/industrial_bridge).

> :warning: On installation with the [ansible playbook](https://github.com/lkzjdnb/H2F_control_deploy) the [config.yaml.j2](/config.yaml.j2) file is used and templated, the [config.yaml](/config.yaml) is unused and only kept as archive.

## Registers
The files [holding_registers.json](/holding_registers.json) and [input_registers.json](/input_registers.json) contains the registers definitions for the [EL41 electrolyser](https://handbook.enapter.com/electrolyser/el41/) as described in the [documentation](https://handbook.enapter.com/electrolyser/el41/el41_firmware/3.6.1/modbus_tcp_communication_interface.html).

The [S7_registers.json](/S7_registers.json) define registers for the control PLC in a [HyET](https://hyethydrogen.com/technology/) HEC compressor, those have been extracted from the provided HMI software ([see compressor_HMI_regs_extract](https://github.com/lkzjdnb/compressor_HMI_regs_extract)).

[meter_holding.json](/meter_holding.json) and [meter_input.json](/meter_input.json) contains the registers definition for a [Finder 7M.38 Power Meter](https://www.findernet.com/en/worldwide/series/7m-series-smart-energy-meters/type/type-7m-38-three-phase-multi-function-bi-directional-energy-meters-with-backlit-matrix-lcd-display/) as described in the datasheet.
