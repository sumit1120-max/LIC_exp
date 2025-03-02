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

   TO perform AC analysis we have to select the ac analysis in the edit simulation command given the values as shown below

   ![Screenshot 2025-02-17 184334](https://github.com/user-attachments/assets/b5b9b5b2-cc27-459c-87d9-27411895f901)
 

   ![1 4](https://github.com/user-attachments/assets/e38ceac5-13a9-46b8-ad3c-efeac570178f)





# Circuit-2:


Now replace the R3 resister with a current source :
connect a current souce of 1mA

<img width="670" alt="1 5" src="https://github.com/user-attachments/assets/f3c98134-6cfc-4c7e-8c4e-f83fc4acd578" />


# DC analysis:

  To perform the DC analysis we have to select the {DC op pnt} in the edit simulation command and run the simulation
   the figure below is the values obtained from the DC analysis

   <img width="472" alt="image" src="https://github.com/user-attachments/assets/96fdac9f-4c40-4170-8c04-0400ca6c4eb8" />


   # Trasient analysis:

  To perform transient analysis we have to select the transient analysis in the edit simulation
   and give the stop time as 5ms and run the simulation .
   and the graph velow shows the transient response of the design

   
   we have to give deg of 180deg to one mosfet and 0deg to the other mosfet
   and ac amplitude 1 for one mosfet and 0 for other mosfet
  ![Screenshot 2025-03-02 130322](https://github.com/user-attachments/assets/9ae919cf-f16c-4df7-ac50-e22cc623c2f2)




 # AC analysis:
 
  <img width="959" alt="image" src="https://github.com/user-attachments/assets/98ec35e3-cac9-41a6-b2cf-5384f4559b01" />




  # Circuit-3:

  Now replace the R3 resister with a Mosfet  :
    Given vp=0.4v and wkt vt=0.36v we got the gate voltage of the new mosfet as 0.76v 

  <img width="597" alt="image" src="https://github.com/user-attachments/assets/341047bc-e16a-4100-8158-de8a16f8dd22" />

 To get the output voltage and vp and current desired value we have to 
 vary the width and length of the new mosfet
![Screenshot 2025-03-02 190203](https://github.com/user-attachments/assets/39f0a14a-c7f1-45ce-b951-6841a94a4e38)


# DC analysis:


<img width="472" alt="image" src="https://github.com/user-attachments/assets/417842be-d7ad-4955-8086-b77ea97d490e" />

 # Transient analysis:
 give ac amplitude as 1 for one mosfet and 0 gor other mosfet 

 ![Screenshot 2025-03-02 123127](https://github.com/user-attachments/assets/431d7132-e2fb-4870-b625-a5334a2e9a9d)

# AC analysis:
<img width="959" alt="image" src="https://github.com/user-attachments/assets/56a10839-f8b8-40e4-8c2f-a01d9dda29f3" />



# DC sweep :
<img width="959" alt="image" src="https://github.com/user-attachments/assets/15f102e5-5ba4-40c5-965c-3c6d8668217b" />


# Result:

1. Circuit-1: 
   - The DC analysis shows that the MOSFETs operate in saturation with balanced drain currents when input voltages are equal.  
   - The transient response confirms proper differential behavior.  
   - The AC analysis indicates moderate gain and common-mode rejection.  

2. Circuit-2:  
   - Replacing the resistor with a current source improves bias stability, as seen in the DC analysis.  
   - The transient response is more stable, ensuring better symmetry.  
   - The AC analysis shows increased gain and bandwidth compared to Circuit-1.  

3. Circuit-3:  
   - The DC analysis confirms that the MOSFET-based current source regulates the tail current effectively.  
   - The transient response maintains signal accuracy with improved performance.  
   - The AC analysis shows higher gain and bandwidth.  
   - The DC sweep analysis validates expected output variations.  

# Inference:  

- The tail current source significantly affects gain and stability.  
- The resistor-based design has lower gain and common-mode rejection.  
- The current source improves circuit stability and differential performance.  
- The MOSFET-based current source provides the best gain and frequency response.




  


   



   

   

   

