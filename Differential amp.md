# Expeiment-3

## Aim:
Design and Analyze the MOS differential amplifier circuit for the following specifcations and Perform DC analysis,Transient Analysis,Frequency response and extract parmeter

VDD=2.2v,P<=2mW,Vicm=1.2v,Vocm=1.25v,Vp=0.4v

#### Differential Amplifier:

differential amplifiers  consist of two transistors M1 and M2, whose sources are joined together. If two transistor are connected to the different voltage input then there current across M1 and M2 are different due to gate voltage.If in case the voltage supply at gate terminal is same then the current through the M1 and M2 are same.This configuration is called "Common Mode input voltage differential Amplifier".WHatever may be the load resistor, the MOSFET M1 and M2 should not go to the Triode region. It should be verified that MOSFET should be in Saturation Region.

For all this circuit we need find out the AC analysis ,Transient analysis And Frequency Response.
# Circuit-1
Components Required: MOSFET(M1,M2 and M3), Resistor,voltage supply's 
![1](https://github.com/user-attachments/assets/74e8e5d1-6cef-40d5-b0ff-d6814bfd2a3f)


Procedure :
Make the circuit connection as given above.
connect the resister at the source terminal of both mosfet 
now calculate the value of Iss as power and vdd is given
and calculate the Id1 and Id2 
now calculate the Rss and Rd 

Now to get the desired values of output voltage and current we have to vary the width and length of both the mosfet
we got L=190nm and W=6.7877um 



![1 2](https://github.com/user-attachments/assets/5282f237-db25-410c-8b19-9d7db7f8c846)



# DC analysis:


   To perform the DC analysis we have to select the {DC op pnt} in the edit simulation command and run the simulation
   the figure below is the values obtained from the DC analysis

![1 1](https://github.com/user-attachments/assets/1ab4f485-9543-42fa-9e90-4e9dc949ebcd)

Here in dc analysis we got the vout as expected and id1 and id2 we got the same 


# Transient analysis:

  To perform transient analysis we have to select the transient analysis in the edit simulation
   and give the stop time as 5ms and run the simulation .
   and the graph velow shows the transient response of the design.

   ![1 3](https://github.com/user-attachments/assets/2d77788f-18f4-4256-a3c5-23f53ab94900)

# AC analysis:
 

   ![1 4](https://github.com/user-attachments/assets/e38ceac5-13a9-46b8-ad3c-efeac570178f)

   

