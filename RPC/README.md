# Codes for Simulations of TIFR Prototype RPC Stack detector (simplified geometry) 
##  RPC Stack detector geometry
This code uses the geometry description stored in GDML files. An example file can be found in https://github.com/basanab/G4_RPC/tree/main/RPC
* The code here gives the simulation for shooting muons (mu+ or mu-) of specified energy distribution and stores the position , momentum , time and paricle id  of each paricle through all the layers for each event. 
## Usage Instructions
- Required: geant4-v11.0.3 
- clone this repository into a folder of your choice (call it repo)
- create a build folder and call `cmake repo`
- type `make`
- There are two ways of running the code:
    -  `./rpc_geom_copy.gdml  ` 
    - This command will show the visualization of the geometry and tracks 
    -  `./rpc_geom_copy.gdml run.mac ` 
    - This command will not show the visualization but run the commands in the run.mac file
- The output is stored in a file named `rpc_500GeV.csv` (or similar) which contains the undigitized positions of the particles crossing the glass_sensitive plate, time, momentum and particle id.
- In this folder one can also find a code used to visualize the events stored in the output file.


