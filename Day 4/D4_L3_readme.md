# Clock tree synthesis TritonCTS and signal integrity

<p align="center">
  <img width="1000" height="" src="../images/152.png">
</p>

<p align="center">
  <img width="1000" height="" src="../images/153.png">
</p>

- So we go for `H-Tree` method
<p align="center">
  <img width="1000" height="" src="../images/154.png">
</p>

<p align="center">
  <img width="900" height="480" src="../images/155.png">
</p>

- After adding buffers 👇
<p align="center">
  <img width="800" height="550" src="../images/156.png">
</p>

### Clock Net Shielding 👇

<p align="center">
  <img width="1000" height="" src="../images/158.png">
</p>
<p align="center">
  <img width="1000" height="550" src="../images/159.png">
</p>

- therefore the clock net is shieled 
<p align="center">
  <img width="800" height="550" src="../images/157.png">
</p>

### Lab Steps to run CTS using TritonCTS

- from the previous labs, run until the placement stage using the commands

```shell
prep -design picorv32a -tag 16-03_17-49 -overwrite
set lefs [glob $::env(DESIGN_DIR)/src/*.lef]
add_lefs -src $lefs

set ::env(SYNTH_STRATEGY) "DELAY 0"
set ::env(SYNTH_SIZING) 1

run_synthesis

init_floorplan
place_io
global_placement_or
detailed_placement
tap_decap_or
detailed_placement
```

- After placement is done, we move on to the CTS stage and we run it using the command `run_cts` which use `TritonCTS` in `OpenROAD`
- The output after CTS stage is 👇
<p align="center">
  <img width="1000" height="" src="../images/173.png">
</p>
<p align="center">
  <img width="1000" height="" src="../images/174.png">
</p>
<p align="center">
  <img width="1000" height="" src="../images/175.png">
</p>

- Verifying if CTS is run properly or not
<p align="center">
  <img width="1000" height="" src="../images/176.png">
</p>

<p align="center">
  <img width="1000" height="" src="../images/177.png">
</p>
<p align="center">
  <img width="1000" height="" src="../images/178.png">
</p>
