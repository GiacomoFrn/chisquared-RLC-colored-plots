# chisquared-RLC-colored-plots
The main feature of this notebook is to plot the chisquared of RLC series data in a colored 2D plot given the fit function of the voltage across the capacity and the best fit parameters (obtained with scipy.optimize.curve_fit).
First you define the chisquared function with two free parametres as "sum of ((data-fit(data, free parameters))/sigma_data)^2".
Then you costrain the domain of the free parameters with numpy.linspace and make the plot with contourf from matplotlib.
