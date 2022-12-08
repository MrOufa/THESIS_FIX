# THESIS_FIX

Changes 08 - 12 - 2022  
## mpc_updater_08122022.m  
Line 155 - 156: if global_power_diff > GLOBAL_IMBALANCE_THRESHOLD changed to  

Lines added above:  
total_r_gen = sum(mpc.gen(iidx_s8760,2))+sum(mpc.gen(iidx_won8760,2))+sum(mpc.gen(iidx_woff8760,2))
