---
title-slide: false
bibliography: references.bib
csl: vancouver.csl
citeproc: true
theme: serif
background-color: "#ffffff"
transition: slide
navigationMode: linear
hash: true
---

:::: {.columns}
::: {.column width="50%"}

## Sample slides
#### PlaceHolderName
#### Universiti Malaysia Perlis
#### [placeholder@email.com](mailto:placeholder@email.com)

<!-- __AUDIO_INTRO_DO_NOT_TOUCH__ -->

:::

::: {.column width="50%"}
![](media/pics/logo1.png)
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide one
**Key Concepts:**
- Energy conservation per @carnot1824.
- $\Delta U = Q - W$
:::

::: {.column width="50%"}
![](media/pics/sample.png)
:::
::::

---

<span class="slide-title" data-title="My Hidden Slide Name"></span>

![](media/pics/wide.jpeg)

---

:::: {.columns}
::: {.column width="50%"}
### The Master Equation
The fundamental relation of thermodynamics:

$$\Delta U = Q - W$$

The work done $W$ is positive when the system expands against an external pressure.
:::

::: {.column width="50%"}
<video data-src="media/videos/sample.mp4" data-autoplay loop muted width="100%"></video>
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Visualizing the Gas Law
**Interactive Model:**

- P, V, and T relationships.
- Use the slider to adjust pressure.
- Observe the phase boundary.
:::

::: {.column width="50%"}
<iframe 
  data-src="media/plots/sample.html" 
  width="100%" 
  height="500px" 
  style="border:none;" 
  scrolling="no">
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 1 Control Chart
**Conditions:** Pressure=200, Temp=338

Analysis of individual measurements against statistical control limits ($UCL$, $LCL$).
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 1 Capability
**Cpk Analysis:**
- USL: 55, LSL: 45
- Calculated $C_{pk}$: 0.82 (Example)

**Assessment:** Machine 1 is **NOT CAPABLE** under these specific environmental stressors.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_capability.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2 Assessment
**Condition:** P=200, T=338

**Metrics:**
- $C_{pk}$ Analysis
- Individual Control Chart
:::
::: {.column width="50%"}
<iframe data-src='media/plots/m2_control.html' width='100%' height='500px' style='border:none;'></iframe>
::: 
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 3 Assessment
**Condition:** P=200, T=338

**Metrics:**
- $C_{pk}$ Analysis
- Individual Control Chart
:::
::: {.column width="50%"}
<iframe data-src='media/plots/m3_control.html' width='100%' height='500px' style='border:none;'></iframe>
::: 
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2 Assessment
**Condition:** P=200, T=338

**Key Findings:**
- Process stability checked via individuals chart.
- $C_{pk}$ determines if tolerance limits are met.
:::
::: {.column width="50%"}
<iframe data-src='media/plots/m2_control.html' width='100%' height='500px' style='border:none;'></iframe>
::: 
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 3 Assessment
**Condition:** P=200, T=338

**Key Findings:**
- Process stability checked via individuals chart.
- $C_{pk}$ determines if tolerance limits are met.
:::
::: {.column width="50%"}
<iframe data-src='media/plots/m3_control.html' width='100%' height='500px' style='border:none;'></iframe>
::: 
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 2 Assessment
**Condition:** P=200, T=338

**Key Metrics:**
- Process stability monitored via individuals chart.
- Calculated $C_{pk}$ for tolerance compliance.

**Result:** Assessment based on $C_{pk} \ge 1.33$ threshold.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m2_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Machine 3 Assessment
**Condition:** P=200, T=338

**Key Metrics:**
- Statistical process control (SPC) chart.
- Process Capability Histogram.

**Result:** Assessment based on $C_{pk} \ge 1.33$ threshold.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m3_control.html' width='100%' height='500px' style='border:none;'></iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide 13: T-Test Analysis (C1)
**Comparison:** Machine 1 vs Machine 2
**Condition:** P=100, T=303

The plot shows the $t$-distribution and the rejection regions at $\alpha = 0.05$.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/ttest_c1.html' width='100%' height='500px' style='border:none;'></iframe>
::: 
::::

---

### Slide 14 & 15: Statistical Result (C1)
- **T-Statistic:** 2.14 (Mock)
- **P-Value:** 0.038 (Mock)

**True Difference Exists?** Yes

---

:::: {.columns}
::: {.column width="50%"}
### Slide 16: T-Test Analysis (C2)
**Comparison:** Machine 1 vs Machine 2
**Condition:** P=300, T=373

Visual representation of the test statistic relative to the critical threshold.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/ttest_c2.html' width='100%' height='500px' style='border:none;'></iframe>
::: 
::::

---

### Slide 17 & 18: Statistical Result (C2)
- **T-Statistic:** 0.45 (Mock)
- **P-Value:** 0.652 (Mock)

**True Difference Exists?** No
