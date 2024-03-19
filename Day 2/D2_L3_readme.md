#  Cell Design and characterization flows


<p align="center">
  <img width="900" height="350" src="../images/39.png">
</p>

- In the each of the step of the flow from RTL to GDSII, the common thing is each step is `cells` or `gates`

<p align="center">
  <img width="300" height="300" src="../images/40.png">
</p>


#### So How do we Model or Characterize these cells or gates?

<p align="center">
  <img width="800" height="450" src="../images/41.png">
</p>

- The standard Cells as shown in the diagram, the same cell can have different size, different functionality, different Vt (threshold voltage) etc..
- And the cells are desinged usnig the following cell design flow
  
<p align="center">
  <img width="800" height="450" src="../images/42.png">
</p>
<p align="center">
  <b>CELL DESIGN FLOW</b>
</p>

<p align="center">
  <img width="1000" height="550" src="../images/43.png">
</p>
<p align="center">
  <b>Inputs for cell design flow(DRC & LVS rules, SPICE models, library & User defined specs)</b>
</p>

<p align="center">
  <img width="1000" height="550" src="../images/44.png">
</p>
<p align="center">
  <b>Design Steps(Ciruit and Layout design)</b>
</p>

## Characterization Flow

1. Read in the Model Files (PMOS, NMOS etc..)
2. Read the extracted spce netlist
3. Recognise the Behavior of the buffers
4. Read the sub-circuits of inverter
5. Attach necessary power sources
6. Apply the stimulus(input)
7. provide output necessary capacitances
8. provide necessary simaultion command ( like transient or dc analysis)

<p align="center">
  <img width="1000" height="550" src="../images/45.png">
</p>
<p align="center">
  <img width="1000" height="550" src="../images/46.png">
</p>
<p align="center">
  <img width="1000" height="350" src="../images/47.png">
</p>

- From 1-8 steps in the form of configuration file is fed to characterization software **`GUNA`**.
This software will generate Timing, noise and power models.

- We obtain Timing, Noise, Power.libs, Function from the GUNA software 
