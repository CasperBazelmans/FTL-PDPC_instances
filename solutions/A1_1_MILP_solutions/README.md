# MILP solutions of the A1 small generated instances

The best solution Gurobi found for each of the 90 instances in `../../A1_1_small_generated_instances`, with the MILP
without (`<instance>_milp_sol.json`) and with valid inequalities (`<instance>_milp_ineq_sol.json`).

Settings: Gurobi 12.0.1, 16 threads on 16 cores of an AMD EPYC 9654 (2.4 GHz) node, 64 GB, time limit 7200 s
(Snellius, October 2026).

Each file has the status (`Optimal`, `Time Limit Reached`, `Memory Limit Reached`), the objective, the lower bound
and MIP gap, and per driver the route with the configuration driven into each stop and its arrival time. Only a
status `Optimal` means the solution is proven optimal. `milp_results.csv` lists all 180 runs, with their status,
bounds, gap and solve time.

No solution was found for F3-6-16-1 and F3-6-16-2 with valid inequalities: these runs hit the memory limit before
Gurobi found one, so they have no file.
