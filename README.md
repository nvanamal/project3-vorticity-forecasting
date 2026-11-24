# Numerical Differentiation Sensitivity and Physics-Enriched Machine Learning for Extreme Vorticity Growth Forecasting in Isotropic Turbulence

A spatiotemporal pilot study by Nagendrababu Vanamala, Ph.D.

## Status
Private working repository. Scientific results frozen; independent execution audit pending. Reported results are transcribed from the researcher's SciServer outputs, not independently reproduced here.

## Study
JHTDB isotropic1024coarse; four 16³ regions, five snapshots, 81,920 velocity vectors. Matched central 8³ subsets yield 10,240 FD2/FD8 tensors and 8,192 transitions. Training: T1→T2, T2→T3, T3→T4 (6,144). Retrospective evaluation: T4→T5 (2,048). No random point-level split was reported. Spatial tests exclude the evaluation region from training.

Best HGB using FD2 features and FD8 growth target: RMSE 2.208505, R² 0.857921. All eight HGB unseen-region evaluations had negative R². FD8 is a higher-order numerical reference, not exact truth.

## Reproduction plan
Obtain authorized JHTDB cutouts following data/README.md; verify canonical data; compute matched derivatives; construct current-time features and growth targets; apply temporal and spatial splits; evaluate baselines and models; bootstrap spatial blocks; regenerate figures. Original scripts and environment lock are pending; no one-command reproduction is claimed.

See docs/artifact_status.md. Do not commit credentials or raw data before checking redistribution terms.
