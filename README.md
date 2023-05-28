# STM32 Nucleo64 C031C6 with Wokwi Simulation

[![Build and Simulate in Wokwi](https://github.com/wokwi/stm32-hello-wokwi/actions/workflows/ci.yml/badge.svg)](https://github.com/wokwi/stm32-hello-wokwi/actions/workflows/ci.yml)

A simple "Hello World" example showing how to run an STM32 project in [Wokwi for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=wokwi.wokwi-vscode).

## Building

We recommend using the [STM32 VS Code extension](https://marketplace.visualstudio.com/items?itemName=stmicroelectronics.stm32-vscode-extension) to build the project. You will also need to install [STM32CubeCLT](https://www.st.com/en/development-tools/stm32cubeclt.html#get-software).

You can also build the project from the command line:

```bash
make
```

Make sure you have the [Arm GNU Toolchain](https://developer.arm.com/downloads/-/arm-gnu-toolchain-downloads) installed.

## Simulation

To simulate this project, install [Wokwi for VS Code](https://marketplace.visualstudio.com/items?itemName=wokwi.wokwi-vscode). Open the project directory in Visual Studio Code, press **F1** and select "Wokwi: Start Simulator".

Once the simulation is running, you should see the text "Hello, Wowki!" in the Serial monitor.
