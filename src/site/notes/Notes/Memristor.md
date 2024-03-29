---
{"dg-publish":true,"permalink":"/notes/memristor/","tags":["research, compiled"]}
---


# Memristor
What is memristor?
Memory and resistor.
$$VG=I$$
V is pressure, voltage
G is condu ctance
I is current

What if the conductance got bigger or smaller as it was used?
The I-V is pinched
![Pasted image 20220812163032.png](/img/user/Attachments/Pasted%20image%2020220812163032.png)
Not storing energy, because the histerisis go through origin point
Facts:
- broad class of resistance-changing devices
- achivable throug diffirent physical mechanizm
	- Phase change, electrostatic, redox, etc
- application
	- Oscillators: high endurance
	- Learners: incremental+low decay. circuit
	- Memory: Fast switching + low decay-> have big energy barrier between stages
	- Optimizers: high endurance + incremental
- does not imply 'non-volatile'
	- have memory--remember their history, life-span
- a lot of memristor out there, you can chose depending on your use case


## TiO2 / TiO2-x memristor
TiO2 and TiO2 have different conductivity. By applying bias voltage, we can push the ion of TiO2-x to TiO2 side, and change the overall resistance.


## From this [youtube](https://www.youtube.com/watch?v=Z5UTRTOfgo4&ab_channel=CITRIS)
1971 Prof Chua predict the existence of fundamental component that 

$dFlux = M dq$

and also,

$v(t) = R[w,i(t)]i(t)$

$dw(t)/dt = f[w, i(t)]$

with $w$ is the state variable 

![Pasted image 20220902163628.png](/img/user/Attachments/Pasted%20image%2020220902163628.png)
- pinched histerysis loop
- cannot store energy or charge. but can store information

![Pasted image 20220902164008.png](/img/user/Attachments/Pasted%20image%2020220902164008.png)
![Pasted image 20220902164200.png](/img/user/Attachments/Pasted%20image%2020220902164200.png)

- TiO2 is semiconductor, but if O goes, + vacant, it become conductor.
![Pasted image 20220902164612.png](/img/user/Attachments/Pasted%20image%2020220902164612.png)
- when we add + voltage, the O vacant diffused (reorganized) to the left. So that the resistance of the total stack is changing.
- Any oxide can be memristor. 

![Pasted image 20220902165013.png](/img/user/Attachments/Pasted%20image%2020220902165013.png)
![Pasted image 20220902165400.png](/img/user/Attachments/Pasted%20image%2020220902165400.png)
![Pasted image 20220902165816.png](/img/user/Attachments/Pasted%20image%2020220902165816.png)
![Pasted image 20220902170323.png](/img/user/Attachments/Pasted%20image%2020220902170323.png)
I vs time and V vs time. The pulse is broaden

![Pasted image 20220902170611.png](/img/user/Attachments/Pasted%20image%2020220902170611.png)


![Pasted image 20220902170730.png](/img/user/Attachments/Pasted%20image%2020220902170730.png)
- state variable in the function of time
- exponential of exponential 

![Pasted image 20220902171005.png](/img/user/Attachments/Pasted%20image%2020220902171005.png)

![Pasted image 20220902171135.png](/img/user/Attachments/Pasted%20image%2020220902171135.png)
![Pasted image 20220902171220.png](/img/user/Attachments/Pasted%20image%2020220902171220.png)

![Pasted image 20220902171554.png](/img/user/Attachments/Pasted%20image%2020220902171554.png)

- We can stop scale down transistor size, just add layers of memristors!.




### Linked notes 
[[003_PJ_home_Study\|003_PJ_home_Study]]
