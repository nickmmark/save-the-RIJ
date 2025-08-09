# save-the-RIJ
should intensivists routinely place central lines in the right internal jugular or save that site for potential future lines?

### Clincial context
Some intensivists and institutions strongly believe that the right internal jugular vein should be preserved in case a patient requires a hemodialysis line in the future. The "Save the RIJ" dogma is based on the premise that it is technically more difficult to place hemodialysis lines in the LIJ (or femoral) vein. Proponents argue that by preserving the RIJ, the "cumulative procedural risk"[1] can be lowered.

I disagree.

If this assumption is true, by prioritizing the LIJ, we are exposing **every** patient who needs venous access to a higher rate of complications, in the hope of reducing the rate of complications for the subset who _might_ need one of these lines later.

I built this interactive web calculator to help clinicians decide for themselves based on thier own assumptions about LEFT vs RIGHT IJ complications as well as institutional rates of CRRT which strategy has the lower cumulative risk to the patient.


![](https://github.com/nickmmark/save-the-RIJ/blob/main/save_the_RIJ.png)

### Save the RIJ? – Central Line Risk Calculator
This interactive web calculator helps clinicians decide whether to place a central venous catheter (CVC) in the right internal jugular (RIJ) immediately or reserve it for potential future hemodialysis (HD) line placement in ICU patients.

Users can enter custom complication rates for CVC and HD line placement by site, as well as the estimated probability of requiring continuous renal replacement therapy (CRRT). The app compares two strategies:

Use the RIJ now:
```
Risk = (CVC complication rate for RIJ) + (Probability of CRRT × HD line complication rate for LIJ)
```

Save the RIJ for HD:
```
Risk = (CVC complication rate for LIJ) + (Probability of CRRT × HD line complication rate for RIJ)
```

Results are expressed as complications per 100 patients and a recommendation is given based on which strategy yields the overall lower risk.




### References
[1]
