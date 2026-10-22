# LNS solutions of the Bustos benchmark instances

The best of 30 single-core LNS runs (LNS_1) for each of the 120 instances in `../../A2_benchmark_instances_transformed`
(`<instance>_lns_sol.json`; lowest objective, ties: lowest seed).

Settings: LNS master 29cf9a1, 1 thread without yards (`--nth 1`), `--maxrem 10 --thres 0.05`, seeds 8001-8030, the
Bustos ALNS time limits (45 / 90 / 135 / 180 s for 25 / 50 / 75 / 100 requests). Snellius genoa (AMD EPYC 9654),
October 2026.

`lns_results.csv` lists per instance the number of runs and the best, mean and worst objective, with the seed of
the best run and the settings. `bustos_C2-T2-W2-100` (8839.14) is a new best-known solution, below the
fragment-based value of 8849.2. LNS 29cf9a1 wrote a route's `fixed` inverted (output only, fixed in 4fd4667). In
these files it has been corrected to `cost_total - wages - emissions`, which is what the objective charged.
