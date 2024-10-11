# ASAP7nm_implementation

**Dataset Updated on 06th October 2024**


Transient Characteristics of CMOS inverter

![ubuntu2  Running  - Oracle VM VirtualBox 03-10-2024 12_04_53](https://github.com/user-attachments/assets/bca59ff2-ef4f-46c9-bb11-a1a7a50fb675)


CMOS Inverter VTC Characteristics
![image](https://github.com/user-attachments/assets/d4a22a68-1444-4e2f-ab1e-c04aea78e2d4)


Rise and fall time are calculated from the transient characteristics graph at 10% and 90% of the max values 

![image](https://github.com/user-attachments/assets/db7caf7f-4834-4c8e-8304-68bed1ea1595)

Then time delay = (rise time + fall time)/2

![image](https://github.com/user-attachments/assets/752704a7-6581-44ad-a4dd-fb9239f269df)

Drain current is output at Vm by KCL whole of the current at output during operation is drain current .


![image](https://github.com/user-attachments/assets/92a18068-d55f-4e6f-9084-60a5068d0caa)

Cg= cgsoxL + cgsoxL = 1.6e-10 x 7e-9 +1.6e-10x7e-9 = 22.40 e-19 F under no bias

![image](https://github.com/user-attachments/assets/ab71d91a-3fbf-4fb4-99a5-b7cc6ab677df)

Under bias Cg = Ig x t / VGS , here VGS = V1 and Ig= I1 The area under current curve gives charge stored within that time period.

![image](https://github.com/user-attachments/assets/d01e797f-58fb-499a-8532-b75b1d89ec7e)

Switching frequency f = 1/T where T is time of one cycle i.e time period between one fall and one rise

When pMOS is ON, nMOS is OFF

When pMOS pulls Vout to VDD
VOH = VDD = 0.7 mV

Minimum output voltage occurs when input is high (Vin = VDD)

When pMOS is OFF, nMOS is ON
The nMOS pulls Vout to Ground

 VOL = 0 V
 
Input Low Voltage,

VIL
– Vin such that Vin < VIL = logic 0

Find on VTC curve the point on the plot where ∂Vin/∂Vout =-1

Input High Voltage, VIH

– Vin such that Vin > VIH = logic 1

Find  point ‘b’ on the plot where slope =-1

VNMH = VOH - VIH = VDD - VIH  VNML = VIL

Av = Change in Vout /change in Vin

Output resistance can be calculated by ohm’s law Von/I2 

Transconductance gm = Av/Rout 

P = PS + Pdyn

– PS: static due to leakage

– Pdyn: dynamic (signal changing) term

Total P = IDDVDD + Cout VDD^2f

Co= Td  /Ro

Leakage current can be calculated from the value of current at 0V input, mark that point on the graph.

## Bootstrapping circuit for sample and hold.

![image](https://github.com/user-attachments/assets/4c884e5e-8c81-4d20-928a-64301979c097)


A bootstrapped circuit is utilized for sample and hold. 

![image](https://github.com/user-attachments/assets/38bf9772-3c2e-48af-b3fc-b6502c00861d)

