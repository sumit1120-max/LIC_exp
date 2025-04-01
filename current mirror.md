 # Current mirror circuit

## **Introduction**

![images](https://github.com/user-attachments/assets/3ae63254-263f-486b-b57c-e95fbe108326)
<p>
A current mirror is an essential circuit in analog electronics that ensures a constant current is copied from one part of the circuit to another. It helps maintain circuit stability by ensuring that variations in load or other external factors do not affect the output current. These circuits are widely used in integrated circuits (ICs) for biasing, active loads, and signal processing, making them crucial in applications like operational amplifiers and other analog systems.
</p>

## **Theory**
A current mirror operates by taking a reference current and duplicating it in another part of the circuit. This is typically achieved using two identical transistors.

For Bipolar Junction Transistors (BJTs):

The first transistor’s base and collector are connected together.

Both transistors share the same base-emitter voltage, ensuring their collector currents remain equal.

For MOSFETs:

The first transistor’s gate and drain are connected together.

Both transistors share the same gate-source voltage, resulting in equal drain currents.


By neglecting the channel length modulation of the two  transistors the drain currents can be given as :



<img width="231" alt="image" src="https://github.com/user-attachments/assets/cc962d81-87a9-4d36-a57a-e7c85e2bcaa1" />





## CIRCUIT DIAGRAM 1
![Screenshot 2025-04-01 192526](https://github.com/user-attachments/assets/d7a18ae3-750f-4732-8729-3336cd872b74)




## Design Question

<p>Design a current mirror circuit which has a gain of AV = -10V/V, power supply of Vdd = 1.8V, and power of P <= 1mW. Find reference current (Iref), output current (Id), and total current (Itotal). Perform DC and AC analysis for mirror ratio 1:1, 1:2.</p>

## Design
-  The MOSFET should be in saturation region 
<table>
<td>V1>V<sub>th</sub></td>
</table>
i.e 0.5>0.366
 
  -  I<sub>taotal</sub>=P/V<sub>dd</sub>
<table>
<td>I<sub>total</sub>=0.55mA</td>
</table>
I<sub>total</sub>=I<sub>ref</sub> + I<sub>p</sub>
I<sub>ref</sub>=I<sub>p</sub>=(I<sub>total</sub>)/2
<table>
<td>I<sub>ref</sub>=I<sub>p</sub>=0.27mA</td>
</table>


## Case 1: L = 180 nm
<img width="593" alt="image" src="https://github.com/user-attachments/assets/336e631a-ef74-44ab-904c-0a45c7557d68" />








### observation :
W = 2.38u.
W/L ratio of M1 and M2 transistors are maintained same .

## Case 2: L = 500 nm


<img width="583" alt="image" src="https://github.com/user-attachments/assets/e8e96bc8-f23b-4837-87aa-6066343dc450" />





### Observation :
W = 6.0649u
W/L ratio of M1 and M2 transistors are maintained same i,e 1:1 .

## Case 3: L = 1 µm

<img width="545" alt="image" src="https://github.com/user-attachments/assets/e865ad60-7bc9-433d-8d42-c644a4ca1d29" />




 W=12.46u.
 W/L ratio of M1 and M2 transistors are maintained same i,e 1:1 .


  ##  W/L Ratio of M1:M2 = 1:2
<img width="471" alt="image" src="https://github.com/user-attachments/assets/f35d69eb-e8f1-41cf-93a3-1aa31d9e8475" />


### Observation : 
Width is kept at 180nm and length were M1:M2 = 2.38u:4.76u
 W/L ratio of M1 and M2 transistors are maintained same i,e 1:2 .

## Transient analysis 





![Screenshot 2025-03-24 020658](https://github.com/user-attachments/assets/a2c43cd8-6813-4cc8-abf4-eeddf8768689)

- **Observation** MaxOutSwing =  1.175V<sub>p-p</sub> 
## AC ANALYSIS





![Screenshot 2025-03-24 021536](https://github.com/user-attachments/assets/0eed4042-a21b-4a33-97ae-8d705ae847a0)


- **Observation** BW = 2.122GHz 




  

 
 # Results
**case1**
LENGTH:180nm, WIDTH:2.38um  W/L = 1:1
**case2**


## Inferences
- Maintaining consistent W/L ratios for the MOSFETs ensures predictable operation of the current mirror.
- As the length (L) of the MOSFETs increases, the width (W) also increases to maintain the same W/L ratio.
- The special case with a W/L ratio of 1:2 shows that the current mirror can be adjusted for different mirroring ratios.
- The total current (I_total) was calculated based on power supply and constraints, resulting in I_total = 0.55 mA, with I_ref and I_p each being 0.27 mA.
- Ensuring MOSFETs operate in the saturation region (V_1 > V_th) is crucial for proper functioning of the current mirror.

## CIRCUIT DIAGRAM 2
![image](https://github.com/user-attachments/assets/7d2cbe1e-88d8-4500-aa88-74487d6b3bc2)

### DC ANALYSIS 

<img width="338" alt="image" src="https://github.com/user-attachments/assets/874a401b-5bd2-470f-82ea-508ab92f668f" />



# Observations:
We can observe that current accross M6 and M3 transistors are almost double because of 1:2 W/L ratio 

- We can observe that current accross M5 and M4 transistors are same because of 1:1 W/L ratio 

### TRANSIENT ANALYSIS 
![image](https://github.com/user-attachments/assets/e7c8540a-1c43-4fba-a4ab-9f1a69178629)


# ObservationA<sub>v</sub>=Vout/V<sub>in</sub>

 = 1.53/0.099 =15.45 v/v


### AC ANALYSIS 

![image](https://github.com/user-attachments/assets/c17724f5-842e-41b3-b787-99a0176e08f5)

# ObservationsB<sub>w</sub>=1.94G<sub>Hz</sub>


## INFERENCE 


 ### Current Accuracy
- **1:1 Ratio**: Higher accuracy owing to identical transistor sizes.
- **1:2 Ratio**: Slight difference observed due to varying transistor widths.
- **Inference**: The 1:1 ratio offers superior current matching.
- **1:1 Ratio**: Utilizes smaller transistors, thus requiring less chip area.
- **1:2 Ratio**: Necessitates larger transistor widths, leading to increased area consumption.
- **Inference**: The 1:1 ratio is more efficient in terms of chip area usage.
- **1:1 Ratio**: Consumes less power due to the use of smaller transistors.
- **1:2 Ratio**: Consumes slightly more power because of the increased transistor sizes.

