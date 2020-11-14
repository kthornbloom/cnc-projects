# WORK IN PROGRESS

# A t-style electric guitar
A Cabronita Telecaster inspired guitar. Built for two TV Jones style pickups.

## Order of operations

### Body Back
 - Prep stock of X-16" Y-18" Z-1.6" (X & Y can be larger if desired)
 - Use a 1/4" tool with at least 35mm of depth
 - Mark a center line down the stock's Y axis, and secure it in the CNC, making sure the line is parallel with the machine. Mark exactly where it sits
 - Set the CNC origin to the center top point of the stock as shown:
![body-back](https://user-images.githubusercontent.com/3322795/99137890-ad088300-25fa-11eb-9278-6cb66926762d.png)
 - Set your spindle speed. For basswood, use the lowest possible setting.
 - Run 1-body-back.nc

### Body Front
 - Flip the stock over so that the neck pocket remains on the same side as before
 - Align the stock with the centerline & set origin in the same place as before:
![body-top](https://user-images.githubusercontent.com/3322795/99137891-ad088300-25fa-11eb-8439-81d980787bdc.png)
 - Run 2-body-front.nc 
 - This program contains 3 operations: Cavity roughing, Cavity finishing, and the outer edges. After each, it will automatically pause with `m0` to give you time to vacuum, adjust, double check, etc. 

### Body Cleanup
 - Use a bandsaw or jigsaw to cut the body from the remaining wood
 - Use a router with flush cut bit (with bearing) to clean the edges, using the CNC cut edge as a guide.
 - Sand as needed
