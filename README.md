# Zhang 2014 NCHCF COMSOL Reproduction Figures

Public figure archive for the automated COMSOL reproduction of Zhang 2014 negative-curvature hollow-core fiber simulations.

This repository intentionally contains only generated PNG/SVG visualization artifacts and a README. It does not contain COMSOL `.mph` models, result CSV/NPZ datasets, reference PDFs, logs, or source scripts.

## Directories

- `figures/root/`: final paper-style figures, QA charts, tracking plots, and baseline plots.
- `figures/field_maps/focus_t6_defaultpml/`: targeted field maps from the focused t=6 um validation run.
- `figures/field_maps/full_defaultpml/`: targeted field maps from the accepted full sweep.

## Recommended Figures

- `figures/root/nchcf_zhang_2014_full_neigs30_defaultpml_paper_fig3_t6_loss_connected_theory.png`
- `figures/root/nchcf_zhang_2014_full_neigs30_defaultpml_paper_fig5_thickness_loss_connected_theory.png`
- `figures/root/nchcf_zhang_2014_full_neigs30_defaultpml_geometry_qa.png`
- `figures/root/nchcf_zhang_2014_full_neigs30_defaultpml_field_validation_contact_sheet.png`
- `figures/root/nchcf_zhang_2014_full_neigs30_defaultpml_fundamental_mode_examples.png`
- `figures/root/nchcf_zhang_2014_full_neigs30_defaultpml_arrow_fem_overlay.png`

## Notes

The field-validation contact sheet is a visual QA panel, not a loss spectrum. Each panel is a selected member of the tracked HE11/LP01-like fundamental branch. The `FUND branch` title marks the fundamental-core branch, while `mode #` is only COMSOL's local eigenmode ordering at that wavelength and is not the ARROW order. The field region intentionally has no extra label overlay, so annotations do not obscure the mode shape.

The fundamental-mode examples figure shows the lowest-loss representative of that tracked branch for each wall thickness.

The ARROW markers in the theory figures are roots of:

```text
lambda_m = 2*t_wall*sqrt(n_silica(lambda_m)^2 - 1)/m
```

They are theory predictions, not fitted FEM peak locations.
