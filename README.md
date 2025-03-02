# LIC_exp
linear integrated circuits
# Experiment-1
Question : given the power p=50uW , perform DC analysis , Transient analysis and AC analysis for the given circuit and check what happens when the width is increased or decreased of each mosfet.
# Design-1:
<img width="761" alt="image" src="https://github.com/user-attachments/assets/197db282-80c8-4b12-bb5e-78640bd3f78a" />


Aim: To find DC operating point find gain using transient analysis and AC analysis.

Components: Mosfet, resistor, dc power supply.

Procedure :
Make the circuit connection as given above.
connect the RD resistor to the drain terminal and dc power supply to the gate terminal and also to the resitor
connect the source to ground 
set the input voltage to 0.6v and vdd to 1.8v.
using the formula of power p=vi
as we know the value of power=50uW and voltage=1.8v
we get current=27uA
by adjusting the value of width and length of the mosfet we will get the current Id 
As length is given 180nm by adjusting we will get width=1.08um


1. DC analysis

   
   To perform the DC analysis we have to select the {DC op pnt} in the edit simulation command and run the simulation
   the figure below is the values obtained from the DC analysis
   
   ![Screenshot 2025-02-17 174813](https://github.com/user-attachments/assets/b9221c03-af3a-4221-a274-6dc18f9150c5)

2. Transient Analysis

   
   To perform transient analysis we have to select the transient analysis in the edit simulation
   and give the stop time as 5ms and run the simulation .
   and the graph velow shows the transient response of the design.

   ![Screenshot 2025-02-17 175139](https://github.com/user-attachments/assets/10b1c6e3-255a-4848-aa02-cc2036cd8cb7)


3. AC analysis
 

   TO perform AC analysis we have to select the ac analysis in the edit simulation command given the values as shown below

   ![Screenshot 2025-02-17 184334](https://github.com/user-attachments/assets/b5b9b5b2-cc27-459c-87d9-27411895f901)

   the Graph shown is the ac analysis

   ![Screenshot 2025-02-17 175437](https://github.com/user-attachments/assets/e0dc0b7d-5dd9-4f7b-9055-76ce8109f34f)


   Result:


    DC analysis

   
    The calculated drain current matches the expected value based on power and voltage, Id = 27uA.
    By adjusting the mosfets channel dimensions where L=180nm and W= 1.08um, The current requirement was succesfully achecived.
    The circuit behaves as expected under DC conditions.


     Transient Analysis

     The transient response graph shows how the circuit behaves over time.
     The response is smooth, with no unexpected delays or distortions.
     The circuit reacts well to changes, confirming its stability.
   
     AC Analysis

     The AC response graph confirms that the circuit remains stable at different frequencies.
     The circuit maintains its performance across the tested frequency range.








     Inference

     the experiment validates that by choosing the correct mosfet dimensiions the drain current can be effectively regulated.
     the width of mosfet significantaly impacts the drain current indicates that any variation in the width directly influences tbe output current . an increas in the width 
     leads to a higher Id and if decreased id also decreases.
     The design works and follwing theortical prediction and it matches the practical value.




# Design-2

![Screenshot 2025-02-18 154637](https://github.com/user-attachments/assets/2e269390-0978-4d0d-b7f5-1f2f2e05e694)


   Aim : To find DC operating point find gain using transient analysis and AC analysis.

   Components : Mosfets M1 and M2 DC power supply.

   Procedure :

   Make the circuit connections as show abovce.
   Connect dc power supply to the gate terminal.
   Connect the source terminal to the ground.
   Set the input voltage by obtaining Vtc curve and Vdd to 1.8 V.

   Using the Formula for Power

   P=vi

   We will get the Values of Id

   Id= 27uA


   we have to get the output current Id for the given circuits by adjusting the values of L & W of both the MOSFETS

   
   by adjusting the value of width and length of the mosfet we will get the current Id 
   As length is given 180nm by adjusting we will get width=0.61um this value of width and length is for both the mosfet


   1.DC Analysis:

   
   To perform the DC analysis we have to select the {DC op pnt} in the edit simulation command and run the simulation
     the figure below is the values obtained from the DC analysis
    
   ![Screenshot 2025-02-18 153133](https://github.com/user-attachments/assets/111fc880-da3b-4b5d-aafe-3835d2d6c381)



   2. Transient Analysis

   
   To perform transient analysis we have to select the transient analysis in the edit simulation
   and give the stop time as 5ms and run the simulation .
   and the graph velow shows the transient response of the design.
   ![Screenshot 2025-02-18 153440](https://github.com/user-attachments/assets/7d66627c-e292-444f-b599-5b3267a617f2)

   


   3. AC analysis
 

   TO perform AC analysis we have to select the ac analysis in the edit simulation command given the values as shown below

   ![Screenshot 2025-02-17 184334](https://github.com/user-attachments/assets/b5b9b5b2-cc27-459c-87d9-27411895f901)

   the Graph shown is the ac analysis

   ![Screenshot 2025-02-18 153641](https://github.com/user-attachments/assets/a82ecce8-26f7-4101-a7e8-b2735f4e6a9a)




   DC sweep:


   ![Screenshot 2025-02-18 153954](https://github.com/user-attachments/assets/2b617a24-66a9-41d9-8617-496d549e74f8)



   gain:
   

   ![Screenshot 2025-02-18 154231](https://github.com/user-attachments/assets/e853f87e-7f95-4139-8f51-8660fe432ed5)

   


   


   RESULTS:

  1.DC analysis
  
  
  The calculated drain current Id aligns with the expected value based on power and voltage  where the value of Id = 27um 
  By fine-tuning the channel dimensions  of both MOSFETs  the desired current was achieved L=180nm and W=0.61um for both mosfets
  The circuit operates correctly within the selected DC parameters 

  
  2.Transient Analysis:

  The transient response graph confirms that the circuit transitions smoothly over time.
  The circuit responds effectively to input variations, indicating stable operation.

  
  3.AC Analysis:

  The AC response graph confirms that the circuit maintains stability over the tested frequency range.
  The circuit functions as expected under AC conditions.


  INFERENCE:


 the experiment validates that by choosing the correct mosfet dimensiions the drain current can be effectively regulated.

  The voltage transfer characteristics  helped to select the correct operating voltage  for saturation.

 M1  has a stronger influence on ID, meaning its width significantly affects the output current  Increase in width increases Id  and vice-versa.
M2 has a smaller influence on ID  meaning changes in its width result in only minor changes  in Id. Increase in width increases ID by small value and vice-versa.






# Expeiment-3

## Aim:Design and Analyze the MOS differential amplifier circuit for the following specifcations and Perform DC analysis,Transient Analysis,Frequency response and extract parmeter

VDD=3.3v,P<=3mW,Vicm=1.65v,Vocm=1.7v,Vp=0.5v
### Components Required: MOSFET(M1,M2 and M3),Load Resistor(to be calculated),voltage supply(VDD and VG)
## Theory:

#### Differential Amplifier:
The differential-pair or differential-amplifier configuration is the most widely used building block in analog integrated-circuit design.It consist of two 
transistors M1 and M2, whose sources are joined together. If two transistor are connected to the different voltage input then there current across M1 and M2 are different due to gate voltage.If in case the voltage supply at gate terminal is same then the current through the M1 and M2 are same (Im1=Im2).This configuration is called "Common Mode input voltage differential Amplifier".WHatever may be the load resistor, the MOSFET M1 and M2 should not go to the Triode region. It should be verified that MOSFET should be in Saturation Region.

This Expereiment is Based on Common Mode Input voltage Differential Amplifier.

This Experiement is conducted in 3 stages.Where common source terminal is connected with

1.Resistor

2.Current source

3.MOSFET 

For all this circuit we need find out the AC analysis ,Transient analysis And Frequency Response.



 

   

