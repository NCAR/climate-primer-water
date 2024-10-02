

Chapter 8: Example Cases
========================


Example Case 1: Delaware River Basin Water System Vulnerabilities under Climate Change
--------------------------------------------------------------------------------------

**Motivation:**

The Delaware River Basin provides drinking water to nearly 15 million people across 4 states, including 3 water supply reservoirs in the upper part of the basin that divert water to New York City. There is a complex governance structure and shared management plan that regulates how water is managed in the basin for human and ecosystem uses, but stressors like drought compounded by land use change, sea level rise, and climate change can expose vulnerabilities in the system. We need to understand how these drivers interact with the water management system to better characterize future water supply risks.

**Question:**

What are the vulnerabilities in the Delaware River Basin water management system under future climate change, land cover change, and sea level rise?

**Considerations:**

*  Water management and reservoir operations planning generally focuses on timescales that are relatively coarse (~weeks) and long (~decades).
*  While snow is important in this basin, topographic gradients are relatively moderate and the basin is generally well-covered by meteorological observations.
*  Spatial units can be coarser or semi-distributed/lumped since we are mostly interested in integrated fluxes like inflows to reservoirs.
*  We need to capture human responses to climate.
*  Since we are focused on water systems vulnerabilities and risks, we likely need to explore a wide range of conditions to truly characterize risk probabilities and uncertainties.

**Approach:**

Because we need to characterize changing risks, we want to explore a wide range of potential conditions. We will therefore target an ensemble approach where we expose our water systems model to a large number of scenarios. We will want to leverage climate data products that span a range of different climate futures and are high-enough resolution to show reasonable estimates for this relatively small basin (~10km or finer), but daily timesteps are reasonable.

**Potential Products:**

*  `LOCA version 2 for North America <https://loca.ucsd.edu/loca-version-2-for-north-america-ca-jan-2023/>`_ : 6-km across North America, daily precipitation and min and max temperature, 1950-2100, CMIP5 SSP 245, SSP 370, and SSP 585, 27 GCMs with up to 10 ensembles per model

* `MACA CMIP5 downscaled data <https://climate.northwestknowledge.net/MACA/>`_ : 4-6-km across the U.S., daily temperature, precipitation, humidity, wind, and radiation, 1950-2099 corrected to Livneh (MACAv2-LIVNEH) or GRIDMET (MACAv2-METDATA), RCP 4.5 and RCP 8.5 scenarios, 20 GCMs




Example Case 2: Compound Flooding Impacts due to Tropical Cyclones under Climate Change
---------------------------------------------------------------------------------------

**Motivation:**

The East Coast U.S. was severely impacted by Hurricane Irene in 2011. The region was primed by an abnormally wet 2 weeks prior to the hurricane's landfall. Heavy rainfall from the hurricane, saturated soils, and storm surge combined to cause severe flooding along the heavily populated U.S. East Coast. See this `Storymap <https://storymaps.arcgis.com/stories/fa28d98081594cf3b2dd9ce3a6d7018b>`_ from the Mid-Atlantic River Forecast Center for a nice overview of the event. Per `Gutmann et al. (2018) <https://doi.org/10.1175/JCLI-D-17-0391.1>`_, hurricanes in the U.S. are becoming slower and wetter under climte change. This shift has the potential to change flooding impacts and amplify (or expose new) vulnerabilities in communities and infrastructure.

**Question:**

What would the flooding impacts of Hurricane Irene look like under a warmer climate? How do the combined effects of antecedent conditions, sea level rise, and hurricane characteristics change under a warmer climate? Do these factors compound or mitigate flooding impacts?

**Considerations:**

*  Flooding impacts, particularly in urban and coastal zones, require hydrodynamic models. These models are generally *high-resolution* (in both time and space), *process complex*, and *data and compute intensive*.

   *  We need high temporal and spatial resolution data products.
   *  Precipitation is most important, but we also need wind and pressure fields (coastal dynamics) and temperature and humidity (antecedent land conditions).
   *  We are limited in the number of simulations we can reasonably do.

*  We are interested in evaluating impacts of an *extreme event*. 

   *  We need a climate data product that represents extreme events. 

**Approach:**

We will follow a **storyline approach** ("physically self-consistent unfolding of past events, or of plausible future events or pathways", `Shepherd et al. 2018 <https://doi.org/10.1007/s10584-018-2317-9>`_), where we seek to understand the driving factors of a particular event and how changes in those factors may alter impacts. We focus on a particular extreme event (Hurricane Irene) and simulate how that event changes under a warmer climate. Since we will be relying on computationally intense impact models, we will follow a more deterministic approach and run a small subset of high-fidelity simulations. We opt for a **dynamical climate downscaling approach** to ensure the extreme precipitation event is well-represented at high spatial and temporal resolution needed for flood impact modeling. Given our storyline focus and desire to do a direct comparison to a simulated event under different global climates (historical and future GHG emissions), we use a **"Pseudo-Global Warming" approach** (`Schär et al. 1996 <https://doi.org/10.1029/96GL00265>`_) to introduce the future climate anomaly to our historical hurricane event simulation to focus on changes in coastal and hydrologic responses due to climate warming.

**Potential Products:**

* `CONUS404-Historical <https://www.usgs.gov/data/conus404-four-kilometer-long-term-regional-hydroclimate-reanalysis-over-conterminous-united>`_ and CONUS404-PGW (coming soon) - CONUS404-Historical is a dynamically downscaled historical weather simulation forced by ERA5 reanalysis product. CONUS404-PGW is a Pseudo-Global Warming simulation based on CONUS404-Historical with anomaly derived using the LENS2 large ensemble (which uses the SSP3-7.0 scenario). Both products incude high-resolution (4-km, hourly) precipitation, temperature, wind, humidity, pressure, radiation fields, among others.

**Similar Examples from the Literature:**

* Marsooli, R., Lin, N., Emanuel, K. et al. Climate change exacerbates hurricane flood hazards along US Atlantic and Gulf Coasts in spatially varying patterns. Nat Commun 10, 3785 (2019). `https://doi.org/10.1038/s41467-019-11755-z <https://doi.org/10.1038/s41467-019-11755-z>`_
* Goulart, H. M. D., Benito Lazaro, I., van Garderen, L., van der Wiel, K., Le Bars, D., Koks, E., and van den Hurk, B.: Compound flood impacts from Hurricane Sandy on New York City in climate-driven storylines, Nat. Hazards Earth Syst. Sci., 24, 29–45, `https://doi.org/10.5194/nhess-24-29-2024 <https://doi.org/10.5194/nhess-24-29-2024>`_, 2024.
* Xue, Z., Ullrich, P., and Leung, L.-Y. R.: Sensitivity of the pseudo-global warming method under flood conditions: a case study from the northeastern US, Hydrol. Earth Syst. Sci., 27, 1909–1927, `https://doi.org/10.5194/hess-27-1909-2023 <https://doi.org/10.5194/hess-27-1909-2023>`_, 2023.

Example Case 3
--------------

Coming soon.


