# LIC_exp
linear integrated circuits
# Experiment-1
Question : given the power p=100uW , perform DC analysis , Transient analysis and AC analysis for the given circuit and check what happens when the width is increased or decreased of each mosfet.
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

![Screenshot 2025-02-17 202320](https://github.com/user-attachments/assets/e216f2bb-7e24-436e-8c86-d88d0840e2d4)

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
    
   ![Screenshot 2025-02-17 200103](https://github.com/user-attachments/assets/e687b280-d032-4260-8452-b10457103dfc)


   2. Transient Analysis

   
   To perform transient analysis we have to select the transient analysis in the edit simulation
   and give the stop time as 5ms and run the simulation .
   and the graph velow shows the transient response of the design.
   
   ![Screenshot 2025-02-17 200245](https://github.com/user-attachments/assets/05c9b471-494c-4c2e-9338-4be22166a47d)


   3. AC analysis
 

   TO perform AC analysis we have to select the ac analysis in the edit simulation command given the values as shown below

   ![Screenshot 2025-02-17 184334](https://github.com/user-attachments/assets/b5b9b5b2-cc27-459c-87d9-27411895f901)

   the Graph shown is the ac analysis


   ![Screenshot 2025-02-17 200501](https://github.com/user-attachments/assets/4071bada-50cb-40a9-a838-694d6bf27e26)




 

   

