---
layout: default
title: optimal-nmr Main page
---
<div style="text-align: center">
<h1> Workshop <br> Optimal Control in MAS solid-state NMR  </h1>
</div> 

October 13-14, 2022, see details in the [**_Workshop_**](/workshop.html){:class="menulink"} section

# Welcome {#my-h1-id}

<div style="text-align: justify" markdown="1">
On this site we summarize our experience with application of optimal control in solid state NMR studies of protein samples. 

Currently, we have developed **tm-SPICE** pulse sequences for the traditional (uni-axial, \\(I_x \rightarrow S_x\\)) magnetization transfer, and 
**TROP** pulse sequences performing transverse mixing (simultaneous \\(I_x \rightarrow S_x\\) and \\(I_y \rightarrow S_y\\)) that allow to systematically enhance
sensitivity by \\(\sqrt{2}\\) for each indirect dimension.
</div>

#### What you find here  {#my-h4-id}

- Pulse shapes for dipolar recoupling experiments in [**_Downloads_**](/sequences.html){:class="menulink"}
- Description how to use these shapes in [**_Experiments_**](/experiments.html){:class="menulink"}

<div style="text-align: justify" markdown="1">
In case of **tm-SPICE** N-CA and N-CO magnetization transfers, we obtain **1.5-times more signal** compared to carefully optimized ramp-CP experiments performed in the range of **MAS frequencies 13-20 kHz**. Our tm-SPICE shapes can be adapted to any MAS frequency in this range. \[3\]

In case of **TROP** transfers, N-dimensional experiments are done in the echo/anti-echo manner using dedicated pulse programs \[4\]. Experiments show
that it is possible to obtain sensitivity gains that go beyond the systematic \\(\sqrt{2}\\) per indirect dimension due to compensation of RF field inhomogeneity.
</div>

<!---
#### What you will find here (we prepare) {#my-h4-id}

- Description of B<sub>1</sub> field in solenoid coils used in typical MAS probes in **B1 fields**
- Introduction to theory behind our optimal control approach in **Theory**
- Description of our numerical tools in **SIMPSON**
-->

#### References  {#my-h4-id}

1. Tosner, Z. *et al.* Radiofrequency fields in MAS solid state NMR probes. *J Magn Reson* 284, 20-32 \(**2017**\). [DOI: 10.1016/j.jmr.2017.09.002](https://doi.org/10.1016/j.jmr.2017.09.002)
2. Tosner, Z. *et al.* Overcoming Volume Selectivity of Dipolar Recoupling in Biological Solid-State NMR Spectroscopy. *Angew. Chemie \- Int. Ed.* 57, 14514-14518 \(**2018**\). [DOI: 10.1002/anie.201805002](https://doi.org/10.1002/anie.201805002)
3. Tosner, Z. *et al.* Maximizing efficiency of dipolar recoupling in solid-state NMR using optimal control sequences. *Sci. Adv.* 42, abj5913 \(**2021**\). [DOI: 10.1126/sciadv.abj5913](https://doi.org/10.1126/sciadv.abj5913)
4. Blahut, J. *et al.* Sensitivity-enhanced multidimensional solid-state NMR spectroscopy by optimal-control-based transverse mixing sequences. *submitted*
