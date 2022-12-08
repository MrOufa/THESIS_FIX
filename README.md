# THESIS_FIX

Changes 08 - 12 - 2022  
## mpc_updater_08122022.m  
Line 155 - 156: 
if global_power_diff > GLOBAL_IMBALANCE_THRESHOLD  
changed to  
if global_power_diff > GLOBAL_IMBALANCE_THRESHOLD && global_power_diff < total_r_gen  
% only curtail if renewables can balance it

Lines added above:  
total_r_gen = sum(mpc.gen(iidx_s8760,2))+sum(mpc.gen(iidx_won8760,2))+sum(mpc.gen(iidx_woff8760,2))

## Generation Flexibility Cut  
Line 465 -> if condition  

Function Added  
Flag_noRES to avoid curtailment throughout  
