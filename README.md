# Global_mean_rising_sea_levels_1993_2023-and-app
Python - Global Mean Rising Sea_levels 1993_2023 + app
Global mean sea level increased by 0.20 [0.15 to 0.25] m between 1901 and 2018. The average rate of sea level rise was 1.3 [0.6 to 2.1] mm yr-1 between 1901 and 1971, increasing to 1.9 [0.8 to 2.9] mm yr-1 between 1971 and 2006, and further increasing to 3.7 [3.2 to 4.2] mm yr-1 between 2006 and 2018 (high confidence). Human influence was very likely the main driver of these increases since at least 1971. Source: IPPC (Intergovernmental Panel on Climate Change), the United Nations body for assessing the science related to climate change, 2023 report https://www.ipcc.ch/report/ar6/syr/

Local UK data on rising sea levels is not usable due to due to the sites not producing climate quality data for sustained periods throughout the year. A UK national report in 2019 for the biannual Global Sea Level Observing System (GLOSS) meeting provides more information about issues with the network, available at https://www.jcomm.info/index.php?option=com_oe&task=viewDocumentRecord&docID=24144.

I will produce a series of line charts and one heatmap using global data.

The dataset was downloaded as txt and required: removing all the initial text, naming (and renaming to facilitate usage) the columns, cleaning, and removing one unnecessary column.

I have been using the "gmsl_variation_with_gia" column as the y-axis data for the global mean sea level rising chart. This column represents the sea height variation (in millimeters) with the Global Isostatic Adjustment (GIA) applied.

I had to translate the "year" column into the x-axis by setting it as the x-axis values for the plot. The "year" column contains fractional years (e.g., 1993.011526), which represent the time points for the sea level measurements. To make the x-axis more interpretable, you have converted these fractional years into datetime objects using a custom function "_frac_year_to_dt."

One might be surprised that the data ranges from -60 to 75. The reason is show more clearly to rising levels by expanding the data range. The fluctuations up and down each day represents the low and high tide occurring every lunar day, or 24 hours and 50 minutes.

In the context of global mean sea level variations, "Global Isostatic Adjustment (GIA)" accounts for the land movement caused by the loading and unloading of ice sheets and glaciers over geological timescales. It is essential to consider GIA when studying long-term sea level changes because the land movement affects the observed sea level measurements at different locations around the world. By applying GIA corrections to the sea level data, scientists can better understand the true global sea level variations and study the effects of climate change on sea levels accurately.

Data credit

GSFC. 2021. Global Mean Sea Level Trend from Integrated Multi-Mission Ocean Altimeters TOPEX/Poseidon, Jason-1, OSTM/Jason-2, and Jason-3 Version 5.1. Ver. 5.1
