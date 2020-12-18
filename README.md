# rFactor <a href="https://www.rfactor.net/"><img src="rFactor2-logo.jpg" /></a> --> ATI <a href="https://www.accuratetechnologies.com/"><img src="ATI_PantoneLogo.png" /></a>
Who says automotive, engineering software is boring?

## Background
<details><p/>

Trade show excitement!
* why
* how
* result
* benefit to business

</details>

## Components
<details><p/>

* rFactor
  * highly realistic car racing simulation software
  * C API to receive telemetry data eg engine, car, lap
* rFactor plugin
  * managed C++ plugin
  * republish telemetry data over UDP
* CANLab
  * CAN bus analysis software
  * C# scripting engine
  * receive telemetry data over UDP
  * republish data over CAN bus
  * control instrument cluster
* VISION
  * realtime ECU (engine control unit) analysis software
  * receive realtime data over CAN bus
  * realtime data visualisation
* Ford Focus instrument cluster
  * CAN connected device
* CAN dbc file
  * contains CAN device addresses and data protocol for:
    * speedometer
    * tachometer
    * water temperature
    * high beam
    * turn indicators (!)

</details>

## Photos
<details>
  <summary>Setup</summary><p/>

  ![setup](ATI-car-annotated.jpg "Setup")<p />

</details>

## Architecture
<details>
  <summary>Overview</summary><p/>

  ![architecture](ATI-car-architecture.png "Architecture")

</details>

## Further work
<details><p/>

* installer for:
  * rFactor plugin
  * CANLab scripts
  * VISION file
* CAN bus setup
* rFactor instructions
  * enabling _hero_ mode

</details>


