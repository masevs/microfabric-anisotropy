## Microfabric Anisotropy from Optical Thin Sections

Quantifying mechanical anisotropy in quartz-rich rocks using structure tensor analysis.

---

## What This Project Does

This repository provides a reproducible workflow that converts standard petrographic thin-section images into quantitative fabric anisotropy metrics.

Instead of manual grain tracing or EBSD, this method uses structure tensor analysis to extract:

- **Coherence (C)** to know local anisotropy intensity  
- **Orientation strength (R)** to know global fabric organization  
- Coherence maps  
- Orientation overlays  
- Rose diagrams  
- Cross lithology comparison plots  

The workflow differentiates deformation domains (mylonite vs quartz veins) using objective, image-derived metrics.

---

## Background

Mechanical anisotropy controls:

- Fracture propagation  
- Shear localization  
- Fault reactivation  
- Borehole stability  

This project demonstrates that optical microstructure can be transformed into quantitative proxies for directional mechanical behavior using open-source tools.

---

## Result

A clear anisotropy hierarchy was observed:

Mylonite >> Quartz vein in schist >> Massive quartz vein

Mylonites exhibit the highest coherence and strongest orientation clustering, consistent with penetrative shear fabric and directional mechanical weakness.

---

## Methods

1. Convert thin section image to grayscale  
2. Compute spatial gradients  
3. Construct 2D structure tensor  
4. Extract:
   - Coherence  
   - Dominant orientation  
5. Compute axial orientation strength (R)  
6. Generate maps and comparative plots  

No manual segmentation required.

---

## Scope and Limitations

- Captures 2D shape-preferred orientation (SPO)  
- Does not measure crystallographic preferred orientation (CPO)  
- Provides a mechanical anisotropy proxy, not a full constitutive model  

Designed as a screening level geomechanical tool.

---

## Repository Structure

- `notebooks/` – Main analysis workflow  
- `src/` – Core functions  
- `figures/` – Representative outputs  

---

## References

Bigün & Granlund (1987) – Structure tensor  
Jaeger et al. (2007) – Rock mechanics  
Mardia & Jupp (2000) – Directional statistics  
Passchier & Trouw (2005) – Microtectonics  

---

## Author

Imas Viestawati S
Geological Engineering
Developed as part of a geomechanics-focused computational portfolio project.
