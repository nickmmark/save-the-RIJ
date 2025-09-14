# save-the-RIJ
should intensivists routinely place central lines in the right internal jugular or save that site for potential future lines?

### Clincial context
Some intensivists and institutions strongly believe that the right internal jugular vein should be preserved in case a patient requires a hemodialysis line in the future. The "`Save the RIJ`" dogma is based on the premise that it is technically more difficult to place hemodialysis lines in the LIJ (or femoral) vein. [Proponents argue](https://pubmed.ncbi.nlm.nih.gov/39755012/) that by preserving the RIJ, the "**cumulative procedural risk**" can be lowered.

I disagree.

If this assumption is true, by prioritizing the LIJ, we are exposing ***every*** patient who needs venous access to a higher rate of complications, in the hope of reducing the rate of complications for the subset who _might_ need one of these lines later.

This is controversial.

I built this interactive web calculator to help clinicians decide for themselves based on thier own assumptions about LEFT vs RIGHT IJ complications as well as institutional rates of CRRT which strategy has the lower cumulative risk to their patients. By expressing the total risk per 100 patients, hopefully we can make informed decisions that mitigate harm.

Try out the calculator yourself [here](https://nickmmark.github.io/save-the-RIJ/)


![](https://github.com/nickmmark/save-the-RIJ/blob/main/save_the_RIJ.png)

### Save the RIJ? – Central Line Risk Calculator
This interactive web calculator helps clinicians decide whether to place a central venous catheter (CVC) in the right internal jugular (RIJ) immediately or reserve it for potential future hemodialysis (HD) line placement in ICU patients.

Users can enter custom complication rates for CVC and HD line placement by site, as well as the estimated probability of requiring continuous renal replacement therapy (CRRT). The app compares two strategies:

`Use the RIJ` now strategy:
```
Risk = (CVC complication rate for RIJ) + (Probability of CRRT × HD line complication rate for LIJ)
```

`Save the RIJ` for HD strategy:
```
Risk = (CVC complication rate for LIJ) + (Probability of CRRT × HD line complication rate for RIJ)
```

Results are expressed as **complications per 100 patients** and a recommendation is given based on which strategy yields the overall lower risk.


### Baseline Assumptions
Based on the [Three Sites Trial](https://www.nejm.org/doi/full/10.1056/NEJMoa1500964), I assume the rate of IJ procedural complications to be about 1-2%. Based on [Sulek _et al_](https://pubmed.ncbi.nlm.nih.gov/10818329/) RCT comparing right vs left sided CVC placement, I assume the risk is double on the left compared to the right (in their study, performed without ultrasound guidance the risk was 10% and 20% respectively). Based on [Oliveros _et al_](https://jintensivecare.biomedcentral.com/articles/10.1186/s40560-020-00481-0), I assume that the risk of an  patient admitted to the ICU requiring dialysis is 10%.



### References
* Gharaibeh _et al_, [Impact of Initial Jugular Vein Insertion Site Selection for Central Venous Catheter Placement on Hemodialysis Catheter Complications](https://pubmed.ncbi.nlm.nih.gov/39755012/), _Journal of Critical Care_ 2025
* Parienta _et al_, [Intravascular Complications of Central Venous Catheterization by Insertion Site](https://www.nejm.org/doi/full/10.1056/NEJMoa1500964), _NEJM_ 2015
* Sulek _et al_, [A randomized study of left versus right internal jugular vein cannulation in adults](https://pubmed.ncbi.nlm.nih.gov/10818329/), _Journal of Clinical Anesthesia_ 2000
* Oliveros _et al_, [Effect of renal support therapy on 5-year survival in patients discharged from the intensive care unit](https://jintensivecare.biomedcentral.com/articles/10.1186/s40560-020-00481-0), _Journal of Intensive Care_ 2020
* Mark & Askin, _Critical Care Time Podcast_, 2025
