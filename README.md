 # Analysis-of-open-loop-and-closed-loop-control-system
## Aim :
  To analyse the open loop and closed loop system having G(S)=1/(S^2+10S+20)  when an unit step input is applied using MATLAB.
## Apparatus Required:
  Computer with MATLAB software
## Theory
  ### Open loop control system
  In this system, the output doesn’t change the action of the control system. It doesn’t have any feedback. It is very simple, needs low maintenance, quick operation, and cost-effective. The accuracy of this system is low and less dependable.
  <img width="652" height="175" alt="image" src="https://github.com/user-attachments/assets/0a9d8129-eb64-40bb-8efd-434edcb2bd5a" />
 ### Closed loop control System
The closed-loop control system can be defined as the output of the system that depends on the input of the system. This control system has one or more feedback loops among its input & output. This system provides the required output by evaluating its input. This kind of system produces the error signal and it is the main disparity between the output and input of the system.
                     <img width="508" height="220" alt="image" src="https://github.com/user-attachments/assets/ad4b9b9e-bf06-4108-a4c0-5320be064b1f" />

Consider a system having plant G(S)=  1/(S^2+10S+20), H(S) = 1(negative unity feedback system) and Controller C(S) = 300.
C(S) and G(S) are in series, 300/(S^2+10S+20)
300/(S^2+10S+20) and H(S) are in negative feedback.
Therefore, Closed loop transfer function, (C(S))/(R(S))=300/(S^2+10S+320)
## Program: 
### Open loop System
```
num[1]
den[1 10 20]
sys=tf(num,den)
step(sys)
```

### Closed loop System
```
num[300]
den[1 10 320]
sys=tf(num,den)
step(sys)
```

## Simulink:
### Open loop system:
<img width="738" height="202" alt="Open loop" src="https://github.com/user-attachments/assets/7a008a18-d1f6-43dc-a137-881f478c2700" />

### Close loop system:
<img width="990" height="195" alt="close loop" src="https://github.com/user-attachments/assets/c441efa3-0c56-41ff-8b15-667b52b3c0a4" />



## Procedure:
	Open MATLAB software
	Open a new script file.
	Type the program.
	Save and Execute the program.
	Analyse the result.
## Output:
### Open Loop System:
<img width="698" height="527" alt="Open loop 1" src="https://github.com/user-attachments/assets/939e44cf-1945-405a-beb1-b1244f4bf422" />

### Closed Loop System:
<img width="695" height="520" alt="close loop (2)" src="https://github.com/user-attachments/assets/5c161d21-d8f9-4afa-8ccc-c2021a283bbe" />

## Result:
Thus the open loop and closed loop system are analysed and the following conclusions are arrived.
### Open loop system
Steady State Error = 0.95 <br>
Settling Time = 2.5
### Closed loop System
Steady State Error = 0.05 <br>
Settling Time = 1.23





