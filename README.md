# rFactor <a href="https://www.rfactor.net/"><img src="rFactor2-logo.jpg" /></a> --> ATI <a href="https://www.accuratetechnologies.com/"><img src="ATI_PantoneLogo.png" /></a>
Who says automotive, engineering software is boring?

## Background
<details><p/>
Trade shows are not the most exciting events.  Automotive trade shows are even less exciting.
Most stands have the vendors dryly demonstrating their products to try and convince you that
it is the best thing since sliced bread.  You have to be very motivated to even approach a
stand, knowing that you will have to endure a sales pitch, which will be the longest 5 mins
of your life! <p/>

We (Accurate Technologies Inc) are in the automotive industry, we do trade shows but we didn't
want to be boring.  What I suggested was using a video game (rFactor) to attract people to our
stand, let them play the game and then engage with them.  rFactor has an API to receive
real time telemetry data, so we could funnel this data through our software (VISION + CANLab)
and display it as the person drove around a track.  Most companies would consider this to be
a bit too 'out there', but not ATI.  It also helps that the owner is a serious petrol head!<p/>

The most difficult part of the software development was getting a C based API (rFactor) to
recognise and load a managed C++ .NET assembly.  Once that hurdle was over, it was relatively
straightforward to receive the telemetry data, republish it and then display it - all in
real time!<p/>

We debuted our racing game at a small, inhouse trade show at a major automotive manufacturer.
We were certainly raising some eyebrows when we setup our 42 inch LCD TV!  Most trade show
exhibition halls are relatively quiet but not this one!  People coming in were greeted to the
sound of a roaring V8 engine, squealing tyres and, quite often, car crashing into armco!
Everyone was staring at use and it wasn't long before we had a queue of people wanting to have a drive.
We were certainly the talk of the show and even our competitors came over the check us out.<p/>

The rFactor setup showed how our products could be used in a fun but 'real world' way.
That people were also able to have 5 mins of light relief was an added bonus :-)
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

## Source Code
Sorry but this is all owned by Accurate Technologies Inc

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


