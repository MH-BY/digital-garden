---
{"dg-publish":true,"permalink":"/notes/references/xu-bayesian-optimization-photonic2022/","title":"Bayesian Optimization of Photonic Curing Process for Flexible Perovskite Photovoltaic Devices","tags":["research, paper,"]}
---



# Bayesian Optimization of Photonic Curing Process for Flexible Perovskite Photovoltaic Devices
#### (2022) - Weijie Xu, Zhe Liu, Robert T. Piper, Julia W.P. Hsu
---------------------------------
- **Link**: 
- **DOI**: 10.2139/ssrn.4172995
- **Zotero Link**: [Bayesian Optimization of Photonic Curing Process for Flexible Perovskite Photovoltaic Devices](zotero://select/items/@xuBayesianOptimizationPhotonic2022)
- **Tags**: #paper
- **Cite Key**: [@xuBayesianOptimizationPhotonic2022]
- **Linked notes**: [[Notes/Paper Annotations\|Paper Annotations]]
----------------------------------
## Abstract
>Photonic curing is a thin-film processing technique that can enable high-throughput perovskite solar cell (PSC) manufacturing. However, photonic curing has many variables that can affect the processing outcome, making optimization challenging. Here, we introduce Bayesian Optimization (BO), a machine-learning framework, to optimize the power conversion efficiency (PCE) of photonically cured MAPbI3 PSCs on ITO-coated Willow Glass. We apply BO with four input variables—MAPbI3 concentration, additive CH2I2 volume, pulse voltage, and pulse length. With the limited experimental budget of 48 conditions, we achieved a champion PCE of 11.42% and predicted 14 new conditions resulting in > 10% PCE. Beyond simple optimization, we examined the relationships between pairs of inputs with twodimensional contour plots and investigated the relative importance of each input to gain insight into photonic curing. We demonstrate that BO is a powerful tool in process optimization and can be adapted to other PSC manufacturing cases.

## Notes

### Need to read the published version
<h1>Annotations
 (1/3/2023, 11:58:35 AM)</h1> 

“We apply BO with four input variables—MAPbI3 concentration, additive CH2I2 volume, pulse voltage, and pulse length.” (Xu et al., 2022, p. 1) 

“photonic curing is a high- throughput process that can convert methylammonium lead iodide (MAPbI3) precursor into a polycrystalline thin film in an ambient environment.[4]” (Xu et al., 2022, p. 2) 

“Photonic curing, or intense pulsed light annealing, uses a flash xenon lamp to deliver intense photon pulses (20 µs to 100 ms) with a broadband spectrum (200 – 1500 nm).[5]” (Xu et al., 2022, p. 2) 

(Xu et al., 2022, p. 2) Bayesian optimization aplications on perovskite. See the references 

“BO has emerged as an efficient optimization tool in the various material science fields,[13–18] including perovskite composition[19] and perovskite solar cell processing.[20]” (Xu et al., 2022, p. 2) 

“an optimization problem, the goal of BO is to find the optimum of a black-box function that is iteratively fitted by a machine learning (ML) regression model; no explainable information about the impact of individual variables on the output is provided.” (Xu et al., 2022, p. 2) 

“We apply the SHarply Additive exPlanation (SHAP) framework[22] to visualize the contribution of each variable to the predicted objective function after the optimization is completed.” (Xu et al., 2022, p. 2) 

“SHAP computes the contribution of each variable to the predicted output and is model-agnostic.” (Xu et al., 2022, p. 2) 

“Briefly, equal molar of nickel nitrate hexahydrate and acetylacetone (0.1 M) were dissolved in 2- methoxyethanol; the solution was stirred overnight and filtered through a 0.2 µm polytetrafluoroethylene (PTFE) filter before spin-coating onto ITO coated WG substrates at 3000 rpm for 30 s. The NiO precursor films were dried at 60 °C for 3 min and then annealed at 250 °C for 30 min to finalize the hole transport layer.[23]” (Xu et al., 2022, p. 3) 

“The MAPbI3 precursors were made according to machine learning output. Stoichiometric PbI2 and MAI were added in N,N- dimethylformamide and dimethyl sulfoxide solution (DMF:DMSO = 9:1 v/v). Later, diiodomethane (CH2I2) was added. The precursors were stirred for at least 2 h before filtering through a 0.2 µm PTFE filter and spin-coating at 4000 rpm for 25 s in an N2-flowing glovebox.” (Xu et al., 2022, p. 3) 

“The ETLs were made by spin-coating 20 mg/mL PC61BM in chlorobenzene at 1200 rpm for 60 s and 0.5 mg/mL BCP in anhydrous ethanol at 4000 rpm for 30 s. F” (Xu et al., 2022, p. 3) 

“We started with a group of experimental conditions picked by Latin Hypercube Sampling (LHS), a pseudo-random sampling method, in the pre- defined input variable space (Table 1).” (Xu et al., 2022, p. 4) 

“The regression model was a Gaussian Process (GP) regression using the Matérn kernel function with an intermediate smoothness parameter v = 5/2, which is a popular kernel choice in BO for intermediate smoothness.[24]” (Xu et al., 2022, p. 4) 

“The length scale l was fitted independently for each 
 process variable by turning on the setting of automatic relevance detection.” (Xu et al., 2022, p. 4) What is this? Length scale l 

“Finally, the prediction results were calculated with the upper confidence bound (UCB) acquisition function to get a new round of experimental conditions.” (Xu et al., 2022, p. 4) 

“We used a BO package called Emukit,[25] and a GP package called GPy[26] in Python.” (Xu et al., 2022, p. 4) 

“For comparing the regression model training after the BO, we first randomly split the entire 48 conditions into 32 training data points and 16 testing data points. We trained and compared several regression models, including Linear, Polynomial, Random Forest, Gradient Boosting, Neural Network, and Gaussian Process Regression. We also trained two ensemble models: Linear ensemble and Random Forest ensemble, both of which include four base learners: Gradient Boosting, Gaussian Process, Random Forest, and Neural Network regression. The best-performing regression model is then fitted with the entire 48 data points. The regression models (except for Gaussian Process) were built with the scikit- learn package. Finally, model interpretation is based upon SHAP analysis with shap package in Python.” (Xu et al., 2022, p. 4) 

“We use LHS to select 16 conditions in our first round (Figure 1a).” (Xu et al., 2022, p. 4) 

“We then fabricated” (Xu et al., 2022, p. 4) 

“the PSCs on WG according to the LHS prescribed values for the four input variables (Figure 1b) and tested their PCEs (Figure 1c).” (Xu et al., 2022, p. 5) 

“In BO, the promising input variables for the next round of data collection are suggested by an acquisition function (Figure 1e).” (Xu et al., 2022, p. 6) 

“We choose UCB as our acquisition policy; UCB balances exploiting the variables leading to the highest PCE and exploring the unknown input regions. This is a mathematic technique to guide how to search the input variable space efficiently while avoiding a trap of local minimum. W” (Xu et al., 2022, p. 6) 

“While BO is easily envisioned by selecting one condition per round and performing multiple rounds until convergence is achieved, we applied a batch optimization method with local penalization [27] to suggest multiple new experimental conditions in every round. In Round 1, 8 of 16 conditions were selected by UCB.” (Xu et al., 2022, p. 6) 

“UCB has a higher success rate than LHS, whereas it is impossible for the OVAT approach to cope with such a complex multi-dimensional space.” (Xu et al., 2022, p. 6) 

“Figure S4 presents the training and testing results of different base learners and ensemble models. Among all the learners, the best learner is the Random Forest ensemble model with four base learners: Gradient Boosting, Gaussian Process, Random Forest, and Neural Network regression[28].” (Xu et al., 2022, p. 7) 

“The Random Forest ensemble's predicted value vs. the ground truth, i.e., the actual PCE measured by the experiment has the highest correlation in the test dataset.” (Xu et al., 2022, p. 7) 

“Spearman coefficient of 0.99 (Figure S5).” (Xu et al., 2022, p. 8) 

“The variable-to-PCE relation trained by the Random Forest ensemble is visualized in Figure 3b: the island features are gone, and its prediction now matches the physical behavior of pulse length.” (Xu et al., 2022, p. 8) 

“By using the particle swarm optimization algorithm,[29] which is a common method to find the global optimum for any regression model, we found the maximum in our variable-to-PCE model located at MAPbI3 concentration = 1.4 M, CH2I2 volume = 172 µL, pulse voltage = 291 V, and pulse length = 21.8 ms, which results in a PCE of 11.18%. This predicted device PCE is within the standard deviation of our experimental results.” (Xu et al., 2022, p. 8) 

“To gain a physical understanding, we apply SHAP to analyze the entire parameter space with our 48 conditions. SHAP, which is a game-theory approach to measuring the contribution of each variable in the model, was recently proposed by Lundberg and Lee as a unified approach to interpreting model predictions.[22]” (Xu et al., 2022, p. 8) 

“SHAP value for a variable provides a measure of the change in the model-predicted PCE due to changes in that variable.[30] Similar to feature importance calculations,[31] the magnitude of SHAP values indicates the importance of the input variables.” (Xu et al., 2022, p. 8) 

“Additionally, SHAP can also provide a quantitative measure of whether the variables positively or negatively affect the model outcome.[32] A positive SHAP value means that the corresponding variable's value will increase the predicted device PCE, and a negative SHAP value means that the corresponding variable's value will decrease the predicted device PCE.” (Xu et al., 2022, p. 8) 

“Pulse voltage has the highest impact on the device PCE” (Xu et al., 2022, p. 8) 

“Figure 4b implies that more CH2I2 and less concentrated MAPbI3 are favorable for higher device performance.” (Xu et al., 2022, p. 8) 

“This result reveals that the optimized precursor formulation, hence film thickness, depends on the processing method even for the same device structure and materials” (Xu et al., 2022, p. 9)