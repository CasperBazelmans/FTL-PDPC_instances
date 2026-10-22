# LNS solutions of the A1_2 medium generated instances

The best of 30 single-core LNS runs for each of the 20 instances in `../../A1_2_medium_generated_instances`
(`<instance>_lns_sol.json`; lowest objective, ties: lowest seed).

Settings: LNS master 29cf9a1, 1 thread with yards (`--yards --nth 1 --nthny 0`), defaults (n_REM 12, T_MAX 0.05),
no `--milp`, seeds 8001-8030, time limit by size: 300 / 600 / 900 / 1200 s for 25 / 50 / 75 / 100 requests.
Snellius genoa (AMD EPYC 9654), October 2026.

`lns_results.csv` lists per instance the number of runs and the best, mean and worst objective, with the seed of
the best run and the settings. LNS 29cf9a1 wrote a route's `fixed` inverted (output only, fixed in 4fd4667); these
instances have no fixed costs, so the files are unaffected.
