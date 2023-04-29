---
{"dg-publish":true,"permalink":"/notes/review-paper-on-perovskite-memristor-1/","tags":["paper, compiled"]}
---


# Literature review

# [[Notes/References/@caoApplicationHalidePerovskites2020\|@caoApplicationHalidePerovskites2020]]
## Biological synaptic function mimicked by memristor:
- Spiking time-dependent plasticity (STPD)
- Paired-pulse facilitation (PPF)
- Excitatory postsynaptic current (EPSC)
- Short-term plasticity (STP)
- Long term plasticity (LTP)

## Physical mechanism of memristor
1. Conductive filaments (CF)
	- mainly caused by ion migration and redox inside the material under external electric field
	- The Resistive switching (RS) 
		1. Can be by electrochemical metallization (ECM)
			- Use metals as top electrode (Ag and Cu)
			- When a positive voltage is applied to the TE, the active metal is oxidized to cation. This cation diffuses downward, passing through the functional layer driven by the positive field. The ions then reduced to metal at the bottom electrode, forming a CF. Thus the memristor switch to HRS to LRS.
			- When a negative voltage is applied, the memristor switch from LRS to HRS.
			- Selecting functional layer to control the formation and rupture of CF
		2. Can be by valence change mechanism (VCM)
			- Metal oxide as a functional layer (for example), when electric field is applied, oxygen ion and oxygen vacancies (Vos) migrate. During SET process (i.e. switching from HRS to LRS), Vos accumulate toward the BE, resulting in the formation of CF of Vos. During the RESET process, Vos combine with Oxygen ions causing the CF to rupture. 
2. Interface types
	- Mainly caused by the change of Schottky barrier at functional layer ($SiO_2$)/insulator. The change of the barrier is usually accompanied by charge trapping/detrapping or anion migration at the insulating layer near the electrode.

##  Development of perovskite memristor
- 1st
	- [Choi et all](https://onlinelibrary.wiley.com/doi/10.1002/adma.201502889), (Au/$CH_3NH_3PbI_3-_xCl_x$/FTO). 
	- Switching voltage less than 1 V
- Best on/off ratio
	- [Sun et al](https://pubs.rsc.org/en/content/articlelanding/2015/TC/C5TC02270C). (ITO/PE-DOT:PSS/$CH_3NH_3PbI_3$/C). 
		- on/off ration 10^4 at read voltage 50mV
	- Kim et al (Ag/$(PEA)_2 Cs_3 Pb_4 I_13$/Pt  )
		- 10^9
- With various metal contacts. highest current switching current ratio.
	- [Zou et al](https://pubs.rsc.org/en/content/articlelanding/2016/TC/C6TC00141F). (Ag/Cu/Ti/Zn/Al)/$CH_3NH_3PbCl_xI_3-_x$/$TiO_2$ compact layer/FTO
	- Switching current ratio as high as 1.9 × 10^9 -> faster read speed, fewer errors, lower power consumption.
- Lead free. low energy consumption.
	- Park et al. Ag/PMMA/$MA_3Sb_2Br_9$/ITO  (MA=$CH_3NH_3$ ; PMMA (Poly methyl methacrylate-> acrylic/plexiglass)

![Pasted image 20220915154930.png](/img/user/Attachments/Pasted%20image%2020220915154930.png)

## The most important properties in memristor are:
 1. Switching speed
 2. Durability 
 3. Retention
 4. Power consumption 

- [ ] #task Finish this review

## How to control conductive filaments
1. Selecting functional layer with excellent performance.
	- Check [this](https://onlinelibrary.wiley.com/doi/10.1002/adma.201400270) and [this](https://pubs.acs.org/doi/10.1021/nn405827t) for Oxide memristors
2. 
2. 
#### Linked notes
[[013_Notes_Research\|013_Notes_Research]]

#important 
