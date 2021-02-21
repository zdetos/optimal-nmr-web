---
layout: default
title: Optimal Experiments
---
# NCA and NCO experiments   {#my-h1-id}


|---|---|
|![NCX pulse sequence](/images/ncx_pulse_sequence.png "NCA/NCO Experiment") | You can download Bruker pulse program using the right-click [here](/sequences/doubcp.zt). |


#### Experimental protocol   {#my-h4-id}

1. **Calibrate RF amplitudes** for all channels using nutation experiment. We need a relation between RF power entered in the spectrometer software (Watts or dB) and the actual nutation frequency (kHz) of such pulse. Note that there is a systematic error due to large RF inhomogeneity - the actual RF amplitude in the coil center is about 10% larger.
2. **Optimize H-N transfer** using <sup>15</sup>N CP MAS experiment. We use ramp-CP with the linear ramp from 70% up to 100% of the RF amplitude applied on the <sup>1</sup>H channel. Contact time of 1 ms is sufficient. This transfer is quite robust towards RF inhomogeneities at moderate MAS frequencies and does not lead to large losses in terms of sample volume pre-selection.
3. Switch to **NCA/NCO experiment**. Set proper values for offsets to be on resonance with the required nuclei (<sup>15</sup>N amides about 120 ppm, <sup>13</sup>C carbonyls about 170 ppm, <sup>13</sup>C alphas about 55 ppm). On Bruker spectrometers, we use the possibility to set the offset during a pulse sequence with the `fq` command.
4. Select proper **RF shapes for tm-SPICE** elements. Adjust their duration and RF amplitudes according to the actual MAS frequency used for the measurement. Our tm-SPICE shapes were calculated assuming duration of a fixed number of rotor periods \\(N_R\\) and a nominal maximal RF amplitude \\(\nu_1^{NOM}\\). Table below explains how to calculate the duration \\(t\\) and the required RF amplitude \\(\nu_1\\) for tm-SPICE shapes generated for 16.5 kHz MAS frequency. Before converting the RF amplitude to Watt/dB, lower it by 10% to compensate the calibration error explained in step 1. 

|                   | Nominal                    |   Actual                   |
|-------------------|----------------------------|----------------------------|
| MAS frequency     | \\(\nu_R^{NOM}\\) = 16.5 kHz | \\(\nu_R\\) = 18 kHz |
| Number of rotor periods | \\(N_R\\) =60 |      \\(N_R\\) = 60        |
| Duration  | \\(t = N_R / \nu_R^{NOM}\\) = 3636.36 &mu;s | \\(t = N_R / \nu_R\\) = 3333.33 &mu;s |
| RF amplitude | \\(\nu_1^{NOM}\\) = 35 kHz | \\(\nu_1 = \nu_1^{NOM} \times \nu_R /  \nu_R^{NOM}\\) |

You should get nice signals. Sometimes, it is beneficial to optimize RF amplitudes of tm-SPICE pulses within \\(\pm\\)1 dB range.