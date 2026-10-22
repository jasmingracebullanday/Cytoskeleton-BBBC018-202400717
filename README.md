# Cytoskeleton-BBBC018-202400717
# Cytoskeleton and Cell Morphology – BBBC018 Lab

**Student ID:** 202400717 
**Phenotype (visual classification):** Prometaphase  
**Image Field ID:** 19468  
**Actin file:** 19468-actin.DIB  
**DNA file:** 19468-DNA.DIB  

**Dataset:** [BBBC018](https://bbbc.broadinstitute.org/BBBC018)  
**Download link:** https://data.broadinstitute.org/bbbc/BBBC018/BBBC018_v1_images.zip  

We used image set BBBC018v1 from the Broad Bioimage Benchmark Collection (Ljosa et al., Nature Methods, 2012).

---

## Brief Fiji Steps

1. Opened `19468-actin.DIB` and the matching `19468-DNA.DIB` in Fiji.
2. Set Measurements: Area, Mean gray value, Shape descriptors, Display label.
3. Used the Freehand Selection tool to outline five intact cells on the actin image.
4. Added each ROI to the ROI Manager (press T) and measured (press M).
5. Saved the Results table as `data/fiji_results.csv` and a screenshot of the measured cells.

---

## Results Summary

| Phenotype    | Image ID | Cells Measured | Mean Area (px²) | Mean Circularity | Mean Aspect Ratio | Mean Actin Signal |
|--------------|----------|----------------|-----------------|------------------|-------------------|-------------------|
| Prometaphase | 19468    | 5              | 3228.4          | 0.660            | 1.160             | 531.8             |

---

## Plots

### Figure 1: Cell Area vs Circularity
![Area vs Circularity](figures/area_vs_circularity.png)

### Figure 2: Actin Intensity
![Actin Intensity](figures/actin_intensity.png)

---

## Answers to Lab Questions

**1. Which specific phenotype did you choose, and what visible features support that choice?**  
I chose Prometaphase. The cells showed condensed chromosomes typical of early mitosis, with the DNA channel displaying compact, brightly stained nuclear material consistent with prometaphase appearance.

**2. Were your five cells mostly round or elongated? Refer to your circularity and aspect-ratio results.**  
The five cells were mostly moderately rounded. The mean circularity was 0.66 (closer to 1 indicates rounder cells) and the mean aspect ratio was 1.16 (close to 1 indicates limited elongation).

**3. What role does actin play in maintaining cell shape and in cell movement (Karp Chapter 9)?**  
Actin filaments form a major part of the cytoskeleton that provides structural support and determines cell shape. Through polymerization, depolymerization, and interaction with myosin motor proteins, actin also generates the forces required for cell movement and migration.

**4. Why can a single fixed fluorescence image NOT show how fast a cell moves?**  
The cells in this dataset are fixed and stained, so the image is a static snapshot of one moment in time. Cell movement and migration speed can only be measured from live-cell time-lapse imaging over multiple time points.

---

## Files Included

- `data/fiji_results.csv` – raw measurements from Fiji  
- `scripts/analyze_cells.R` – R analysis script  
- `results/cell_summary.csv` – numerical summary  
- `figures/area_vs_circularity.png`  
- `figures/actin_intensity.png`
