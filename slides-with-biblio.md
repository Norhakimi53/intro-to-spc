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

<audio id="bg-music" src="media/audio/sb.m4a" loop></audio>

<div id="audio-credit"
     style="position: absolute; bottom: 40px; right: 20px; font-size: 0.6em; opacity: 0.6;">
  Music: “Adrift” by Scott Buckley (CC BY 4.0)
</div>

<script>
  document.addEventListener('DOMContentLoaded', () => {
    const audio = document.getElementById('bg-music');
    const credit = document.getElementById('audio-credit');

    // hide credit by default
    credit.style.display = 'none';

    const test = new Audio('media/audio/bgm.mp3');

    test.addEventListener('canplaythrough', () => {
      // bgm.mp3 exists → use it, keep credit hidden
      audio.src = 'media/audio/bgm.mp3';
    }, { once: true });

    test.addEventListener('error', () => {
      // bgm.mp3 missing → sb.m4a will play → show credit
      credit.style.display = 'block';
    }, { once: true });

    document.addEventListener('click', () => {
      if (Reveal.getIndices().h === 0) {
        audio.volume = 0.5;
        audio.play();
      }
    }, { once: true });

    Reveal.on('slidechanged', (event) => {
      if (event.indexh > 0) { audio.pause(); }
      else { audio.play(); }
    });
  });
</script>

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

---

### Slide 19: Factor Analysis - Pressure (P)
**Factor:** Pressure
**P-Value:** 0.0000

**Significant Effect?** Yes

---

### Slide 20: Factor Analysis - Temperature (T)
**Factor:** Temperature
**P-Value:** 0.0721

**Significant Effect?** No

---

### Slide 21: Factor Analysis - Interaction (P*T)
**Factor:** Pressure $\times$ Temperature
**P-Value:** 0.3002

**Significant Effect?** No

---

:::: {.columns}
::: {.column width="50%"}
### Slide 22: Interaction Plot
**Machine 1 Resistance**

This plot visualizes how the effect of Pressure on Resistance changes across different Temperature levels. Non-parallel lines indicate a potential interaction effect.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/m1_interaction.html' width='100%' height='500px' style='border:none;'></iframe>
::: 
::::

---
# Bibliography
<div id="refs"></div>
