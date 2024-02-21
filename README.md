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

If wokwi complains about a missing firmware, you may need to tell cmake to generate a debug build. Press **F1**, select "CMake: Select Configure Preset", and choose "debug".

Once the simulation is running, you should see the text "Hello, Wowki!" in the Serial monitor.

### Debugging

You can also debug the simulated project using the built-in debugger in Visual Studio Code. To do that, follow these steps:

1. Configure cmake to generate a debug build by pressing **F1**, selecting "CMake: Select Configure Preset", and choosing "debug".
2. Press **F1** again and select "Wokwi: Start Simulator and Wait for Debugger".
3. Press **F5** to start the debugger.

The debug configuration is already defined in the [.vscode/launch.json](.vscode/launch.json) file. For more information, see the [Wokwi for VS Code documentation](https://docs.wokwi.com/vscode/debugging).
