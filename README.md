For investigating saturation levels against various instrument parameters.

To use, firstly go into get_saturation.py and change line 10 to match your machine setup.

Then you can create a script similar to ndfilt_vs_dit/run_ndfilt_vs_dit_COARSE.py
This will run the simulations under the different instrument variations and save the number of saturated pixels for each variation to disk.

Then you can create a jupyter notebook similar to ndfilters_vs_dit.ipynb, to load in the results and plot.