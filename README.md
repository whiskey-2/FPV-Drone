# FPV-Drone
The idea stemmed from the need of a cool project that combined electrical and mechanical engineering, for me and my cousin. With how popular kits are for FPV drones, we decided to make our own chassis and deal with the integration issues that may arise from that...

## Engineering Overview: My Role in the Project
I took the role of designing the chassis, mounts and arms; whereas we both assembled the drone together. The arms were designed using a topology study completed in Solidworks, that reduced the bulk mass of the arms and created an organic shape for the arm that would still withstand the load being applied to it. That was the prototype design for the drone. 

**Topology Simulation Results:**

The front and rear arms had their mass reduced by 92% while retaining full stiffness. An 80% reduction was selected to attempt to account for the material differences of 3D printed and bulk material.

**Boolean Design Method:**

The chassis of the drone was taken from a GrabCAD project designed for proper Epoxy infused Carbon Fiber parts. To make adjustments to the existing files, the chassis was taken into Blender to use it's Boolean and Modeling tools and thus make changing bolt positions and a thicknesses a simple task. Furthermore, it made modifying the organic motor arms more flexible and refined, allowing for more nuanced adjustments.

**3D Printing the Frame:**

The frame of the drone required a material stronger than the PLA I am used to, so I explored potential filaments that my printer could handle. The final result was the use of either a Carbon-Fiber or a Fiberglass infused PETG composite. The Fiberglass, while stiffer was significantly harder to print reliably and was also more expensive, which led us to settle for PETG-CF. We opted for a 15% infused mix, and started the printing process. This was a multi-phase process, as while the print bed could fit the entire frame, the prints were failing often. 

After some troubleshooting, it was found that the filament is rather hygroscopic. Drying the filament before a print was found to be ineffective due to the print time, as such a filament dryer with a feed tube was employed to keep the filament dry and allow for properly fused layers.

**Assembly:**
The bottom region of the frame was assembled first, starting with the motors on the arms, the arms to the lower base and then to the upper base, where they were sandwiched together. We used M3 bolts with sealing nuts on the end to make sure the frame would remain assmebled, but not require adhesives for the assembly. The FPV camera mounts were then added along with the camera. The flight control, VTX as well ELRS receivers were all placed in their respective locations. The top plate was screwed into the place, and we now had an assembled drone, with the FPV part working.

**Testing:**
With the drone assembled, we took started trying to connect the controller to the drone, without any propellors attached. The controller originally wouldn't pair to drone's receivers, and the only way to control the motors was through the firmware app for the Flight Controller. We updated the firmware for the controller and set it to automatically detect the range the drone is supposed to send, and it finally detected the drone. We set an arm/disarm button for the motors and fired it up. As soon as the motors were armed, despite the fan speed arm being set to the lowest setting, the arms went full speed, shaking the drone so violently it rocked from side to side on the legs. The legs turned out to be uneven, a discovery made on the spot, and the drone bounded onto one arm, breaking it, and then onto the opposite breaking it again.

**Outcome:**

With the arms now broken, the drone is now out of commission, but there is alot to learn from the project and how it went. First off, let me talk about the reason for the failure and next steps. The arms breaking is a combination of two factors. First, the Generative Design was printing elements too thin to realistically support this, and it created a point of failure that I did not recognize, where the motor mount attachement point to the rest of the arm was incredibly thin. Second, the arms used during the assembly were printed with the filament still a little wet, the filament drier being used was not able to get up to temp, and failed halfway through, creating bubbles in the print and reducing layer adhesion and coherence, this reducing overall strength and stiffness. These factors combined had the drone fail upon impact with the ground. The next steps are to find a different way to reduce mass for the arms, or modify the settings for the topology study to ensure the attachement of the mount is wide. We also need to find why the arming of the motors automatically sent it to max power.
