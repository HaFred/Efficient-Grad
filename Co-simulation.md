# Co-simulation using SCALE-Sim and DRAMSim

## Prerequsites
- [x] Customize SCALE-Sim to emit the cycle-discrete traces (such customization I shall call it non-vanilla version)
- [x] Customize DRAMSim3 for script-based recording needed

## Steps
* Define the top config & network topology files in SCALE-Sim
* Run SCALE-Sim `scale.py` to emit the DRAMSim3 format traces (both DRAM & SRAM traces contained)
* Use the DRAM traces for DRAMSim3 simulation. Just run the `recursive.sh`
* (Optional) Matplotlib plotting using the csv files dumpped by `recursive.sh`. Actually I appended the bash support for matplotlib in `recursive.sh` in the commit of Apr29
