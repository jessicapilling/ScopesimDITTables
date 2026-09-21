Using the AutoExposure mode of Scopesim to find DIT times for different observing modes of Metis. 

The WCU is not changed from its defaults, which are printed in "check_wcu_defaults.ipynb". When I ran this, every mode used the blackbody lamp at 1000 K.

The jupyter notebooks output csv files, which are then formatted by format_table.ipynb, which turns them into markdown tables with nicer column names and rounding of numbers to a nice number of decimal places. (This requires the "tabulate" python package.)

When DIT < MINDIT, the "MINDIT Hit" column is set to True, and the value in the "DIT" column is MINDIT.
In this case, a value is also added to the "Attempted DIT" column, which was the original
calculated DIT output by the AutoExposure object. This code extracts the calculated DIT from the warning string that ScopeSim prints. I think this output is set to 3 decimal places, so sometimes the attempted DIT will be 0.000s. 
