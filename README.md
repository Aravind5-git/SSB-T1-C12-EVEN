# SSB-T1-C12-EVEN
AIM:

To write a program to perform SSBSC modulation and demodulation using SCI LAB and study its spectral characteristics

EQUIPMENTS NEEDED:

.Computer with i3 Processor

.SCI LAB

ALGORITHM:

Define the Function: Specify the function you want to simulate. For example, f(x)=sin⁡(x)f(x)=sin(x) or any other function.
Generate Sample Points: Decide on the range and the number of sample points. Generate these sample points within the desired range.
Evaluate the Function: Compute the function values at each of these sample points.

PROCEDURE:

1.Refer Algorithms and write code for the experiment.

2.Open SCILAB in System

3.Type your code in New Editor

4.Save the file

5.Execute the code If any Error, correct it in code and execute again

6.Verify the generated results

PROGRAM:
```
Am=11.5;
fm=426;
Ac=23;
fc=4260;
fs=42600;
t=0:1/fs:2/fm;
m1=Am*cos(2*3.14*fm*t);
subplot(4,1,1);
plot(t, m1);
cl=Ac*cos(2*3.14*fc*t);
subplot(4,1,2);
plot(t,cl);
m2=Am*cos(1.57-(2*3.14*fm*t));
c2=Ac*cos(1.57-(2*3.14*fc*t));
a = cl.*m1;
b = c2.* m2;
c = a + b;
subplot(4,1,3);
plot(t, c);
d=a-b;
subplot(4,1,4);
plot(t, d);
```
TABULATION:

<img width="1018" height="1599" alt="image" src="https://github.com/user-attachments/assets/d76b3b2b-0523-4bf4-85fa-65121dfa0c80" />


OUTPUT GRAPH:

<img width="610" height="460" alt="image" src="https://github.com/user-attachments/assets/bf550d19-2b08-48a3-867d-03e2e22957d5" />

RESULT:

<img width="1600" height="1406" alt="image" src="https://github.com/user-attachments/assets/83b2306d-48c2-475e-a7a2-45da24cbbe8e" />
