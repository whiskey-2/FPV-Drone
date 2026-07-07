# FPV-Drone
The idea stemmed from the need of a cool project that combined electrical and mechanical engineering, for me and my cousin. With how popular kits are for FPV drones, we decided to make our own chassis and deal with the integration issues that may arise from that...

## Engineering Overview: My Role in the Project
I took the role of designing the chassis, mounts and arms; whereas we both assembled the drone together. The arms were designed using a topology study completed in Solidworks, that reduced the bulk mass of the arms and created an organic shape for the arm that would still withstand the load being applied to it. That was the prototype design for the drone. 

**Topology Simulation Results**
The front and rear arms had their mass reduced by 92% while retaining full stiffness. An 80% reduction was selected to attempt to account for the material differences of 3D printed and bulk material.

**Boolean Design Method**
The chassis of the drone was taken from a GrabCAD project designed for proper Epoxy infused Carbon Fiber parts. To make adjustments to the existing files, the chassis was taken into Blender to use it's Boolean and Modeling tools and thus make changing bolt positions and a thicknesses a simple task. Furthermore, it made modifying the organic motor arms more flexible and refined, allowing for more nuanced adjustments.

**3D Printing the Frame**
The frame of the drone required a material stronger than the PLA I am used to, so I explored potential filaments that my printer could handle. The final result was the use of either a Carbon-Fiber or a Fiberglass infused PETG composite. The Fiberglass, while stiffer was significantly harder to print reliably and was also more expensive, which led us to settle for PETG-CF. We opted for a 15% infused mix, and started the printing process. This was a multi-phase process, as while the print bed could fit the entire frame, the prints were failing often. 

After some troubleshooting, it was found that the filament rather hygroscopic. Drying the filament before a print was found to be ineffective due to the print time, as such a filament dryer with a feed tube was employed to keep the filament dry and allow for properly fused layers.

**Assembly**
