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

<details>
  <summary>Instrument Cluster</summary><p/>

  ![instrument cluster](Ford-Focus-instrument-cluster.jpg "Instrument Cluster")<p/>

</details>

## Architecture
<details>
  <summary>Overview</summary><p/>

  ![architecture](ATI-car-architecture.png "Architecture")

</details>

## Screenshots
<details>
  <summary>rFactor</summary><p/>

  ![rFactor](rFactor-01.jpg "rFactor")
  ![rFactor](rFactor-02.jpg "rFactor")
  ![rFactor](rFactor-03.png "rFactor")
  ![rFactor](rFactor-04.jpg "rFactor")

</details>

<details>
  <summary>VISION</summary><p/>

  ![VISION](VISION-Demo-Screen-Cal-Changes.png "VISION")
  ![VISION](VISION-MultiGraph.png "VISION")
  ![VISION](VISION-Screen-OBDII-Data.png "VISION")

</details>

<details>
  <summary>CANLab</summary><p/>

  ![CANLab](CANLabDisplays_576x408.png "CANLab")
  ![CANLab](CANLabScope_576x374.pn "CANLab"g)
  ![CANLab](CANLabSend_576x378.png "CANLab")
  ![CANLab](CANLabScript_576x472.png "CANLab")

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


