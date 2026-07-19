# DIY SlimeVR Tracker (Cheesecake Blueberry Variant - `BB-LSM6DSV`)
Our main OpenPaw trackers are a close variant of [Sorakage033's SlimeVR Cheesecake Blueberry trackers](https://github.com/Sorakage033/SlimeVR-CheeseCake) with a couple specific changes for reliability and asthetics.

## Changes from Sorakage033 Cheesecake Blueberry

### PCB Changes:

1. The power switch on the PCB has been changed to a stronger version to prevent it easily breaking off with minimal force when assembling trackers. They are more expensive, but we believe are very worth the additional cost for the robustness they add!
2. The USB-C port has been changed out for a light-blue variant to add to the "blueberry" asthetic.
3. The battery connector has been changed to be JST-2.0mm connectors for consistency and compatibility with existing batteries on the market. On most (or hopefully all) boards that we sell it should come with a nice dark blue/purple JST connector to match the overall blueberry asthetic.
4. You can now solder a battery directly on the bottom of the board to the new battery pads, this should make it simpler for first time solderer's to attach their own batteries that might not have JST connectors.
5. Adjust pad & trace size for ground on TP4057 to improve heat dissipation to reduce the amount of heat generated when battery is very low on charge. We don't want you to burn your paws, but sadly were not able to fix this issue fully. In a later revision we plan to replace the TP4057 with a smarter switching charging chip to prevent the issue with excess voltage being dissipated as heat.
6. Swapped out minor components that were low on stock to defaults that should always be in stock without any issues!
7. Changed the soldermask to be cuter and to include a QRCode to take you directly to our documentation site explaining how to assemble/build the trackers!
8. Removed the BMM350 Magnetometer & circuitry until a proper firmware can be designed that implements SoftFusion between the LSM6DSV and BMM350 Magnetometer for better sensor fusion. Until then we decided it was best to not leave unpopulated components on the board, but we will do our best to get the adjusted firmware into the main branch for SlimeVR!
9. Likely a few others that I am forgetting here, but that should be the bulk of em!

### 3D Print file changes:

We have painstakingly recreated CAD files for every 3d model so that you can modify them as you see fit should you want to! These closely match the original cases/mounts with a few key differences.

Tracker Case:

1. The default screw hole type has been changed to use "self-tapping" M2 screws to make assembly much more simple! You no longer need to use heat-set thread inserts or embed M2 nuts into the board/charging dock. This should provide the same security for mounting the boards without the hassle of previous methods!
2. The slide mounts rail guides now have a deeper "clip" for more secure attachment.
3. (pending) The top of the case has been adjusted to better show the charging LED status

Charging Dock:

1. The CAD model is configurable for 6, 8, and 10 tracker variants (10 tracker board file coming soon).
2. Charging Dock base will no longer have print issues for the screw lips as they are now tapered to prevent printers extruding filament in mid-air.
3. Charging dock top has been adjusted to use self-tapping screws the same as the Tracker case for simplified assembly!

Slide Mounts:

1. Adjusted the size of the strap holes to better fit thicker straps like VyroVR and Mochi comfort straps! They have also been adjusted to fit 30mm tracker straps better instead of using the old 50mm wider straps. The gaps are now fully configurable, so feel free top hop into the design file and adjust them to your liking!
2. Adjusted the design to work better with PLA in case users do not have PETG available
3. Adjusted the size/positioning/shape of the clip tabs for a more secure and stronger fit.
4. Adjusted the slide positioning/fit slightly to have better grip and prevent wiggling.