.. vim: syntax=rst

**I. Introduction » What is Precipitation Estimation (QPE)?**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The term Quantitative Precipitation Estimation, or QPE, refers to the
estimation of observed precipitation.

|24h QPE|

This is different than a forecast of precipitation which is referred to
as a Quantitative Precipitation Forecast, or QPF.

|48 h QPE|

You may wonder why precipitation is only an estimate if it is
“observed.” Observed precipitation is only an estimate because the tools
used provide inexact approximations of the actual magnitude and
distribution of precipitation.

**I. Introduction » QPE Methods and Tools**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Radar is a remote sensing QPE tool with excellent spatial and temporal
resolution. However, radar coverage may be inconsistent from place to
place and from storm to storm.

|Illustration of radar, satellite and rain gauges sensing a convective
cloud system.|

Satellite is another remote sensing QPE tool, but with much coarser
resolution than radar.

|image1|

Even rain gauges, which are ground-based measurements, are subject to
errors and cannot resolve the spatial detail of precipitation patterns.

|image2|

A precipitation climatology is sometimes used to augment the estimates
of observed precipitation. This can be very useful in regions where
precipitation distribution, and the ability to observe it, is greatly
affected by terrain features.

**II. Remote Sensing of QPE**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Precipitation accumulation is routinely derived from radar and satellite
observations. Despite the inconsistencies in radar-derived precipitation
from location to location and from season to season, radar guidance is
considered superior to satellite guidance of QPE in many areas. This is
mainly due to the superior resolution in both space and time and often
better quantitative guidance.

|Radar-derived Total Accumulation|

Topics in this section include the relationship between drop size
distribution, the Z-R relationship, and derived rainfall; the impact of
snow on radar-derived estimates, the potential QPE improvement with
polarimetric radar, radar coverage issues, and the concept of radar
climatology. A brief summary of issues regarding satellite-derived QPE
will follow the radar sections.

**II. Remote Sensing of QPE » Reflectivity-Rainfall Rate (Z-R) and Drop Size Distribution (DSD)**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Radar reflectivity (Z), expressed in units of dBZ, is used to compute
rainfall rates (R) in mm/h using a reflectivity to rainfall rate
relationship. This is known as the Z-R relationship. Rainfall rates then
get integrated over time to produce accumulation for various time
periods.

|Hybrid Reflectivity near LaCrosse, WS 0057 UTC 19 Aug 2007|

|Instantaneous Radar-derived Rainfall Rate near LaCrosse, WS at 0057 UTC
19 Aug 2007|

|Storm Total Radar-Derived Rainfall Accumulation near LaCrosse, WS 0057
UTC 19 Aug 2007|

The relationship between reflectivity and rainfall rate, and thus the
Z-R relationship, varies with time, location, and season. Hydrometeor
properties that influence the Z-R relationship include size,
concentration, and phase. Accuracy of derived rainfall rates is further
impacted by the presence of non-hydrometeors, and whether the radar is
sampling a region that is representative of precipitation reaching the
ground.

|Convective storm illustration with close up of hydrometeor sizes|

|Convective storm illustration with close up of hydrometeor
concentration|

|Convective storm illustration with close up of hydrometeor phases|

|Convective storm illustration with close up of non-hydrometeors|

|Convective storm illustration with hydrometeor sampling by radar|

Hydrometeor shape, which is related to hydrometeor size and phase, is
also important information for understanding the relationship between
reflectivity and precipitation rates. Large liquid drops are more oblate
in shape than smaller ones. For horizontally-polarized radars like the
WSR88-D, greater horizontal diameters reflect more energy back to the
radar. This results in greater derived rainfall rates.

|Drop shapes as a function of size|

Even relatively small 13-mm (half-inch) diameter hailstones contribute
greatly to radar reflectivity. That’s why the presence of hail results
in anomalously high derived-rainfall rates. This anomaly is typically
minimized through use of rainfall rate thresholds.

**In Depth: Reflectivity Factor, Z**
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**Z = ∫ N(D) D\ 6 dD**
^^^^^^^^^^^^^^^^^^^^^^

| **Z** = reflectivity factor
| **D** = drop diameter
| **N(D)** = number of drops of given diameter per cubic meter

This equation is presented to explain the sensitivity of reflectivity
factor, Z, to drop diameter. Because the drop diameter is raised to the
6th power, small changes in drop diameter result in very large changes
to Z. And large changes to Z result in large changes to derived rainfall
rates.

Drop size distribution (DSD) refers to the size and concentration of
drops in a volume, say a cubic meter. Here we show two DSDs.

|DSDs with equivalent reflectivity but different rainfall rates|

The radar is more sensitive to the horizontal diameter of the
hydrometeors than it is to the concentration of hydrometeors. Therefore,
a small number of large hydrometeors can result in the same reflectivity
value as a very large number of smaller drops. But the DSD on the right
is producing greater rainfall rates. The two DSDs should therefore be
represented by different Z-R relationships.

The DSD can vary significantly and quickly in both space and time. This
means that it may be appropriate to have more than one Z-R relationship
in effect at the same time. As of this writing, the NOAA National Mosaic
and Multisensor QPE (NMQ) radar precipitation product can utilize
numerous Z-R relationships based on atmospheric conditions.

Here we have a region with a squall line that most likely has a DSD
consistent with convective rainfall. Nearby stratiform precipitation
will exhibit a different DSD and should be associated with a different
Z-R relationship than the convective area. As the precipitation system
moves, the Z-R relationship at any one location should change with time.

|Reflectivity Image at 2126 UTC 15 November 2008|

**II. Remote Sensing of QPE » Reflectivity and Snow**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

As snowflakes begin to melt, a coating of water can make them “appear”
as very large raindrops to the radar. This can cause very high
reflectivity and overestimated rainfall rates at the ground below where
the radar is sampling the melting layer aloft.

|Radar and melting snow|

Pure snowflakes and crystals violate the assumption of liquid
hydrometeors that go into the Z-R equation. However, several research
institutions are working on radar-derived snowfall including Z-S, or
reflectivity snowfall rate relationships.

**II. Remote Sensing of QPE » Precipitation Estimates with Dual Polarimetric Radar**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Advances are made in radar technology every year. As this lesson is
being developed the most promising with respect to precipitation is dual
polarized radar, or polarimetric radar.

|Sample data from dual-polarimetric Radar|

A network of polarimetric radars promises to alleviate some of the
errors associated with the phase, size, and distribution of
hydrometeors. Ultimately, this means the problems associated with
inappropriate Z-R conversions should be minimized.

Excellent training on precipitation measurement using polarimetric radar
is available from NOAA’s WDTD. We will not repeat those lessons here,
but we strongly encourage you to review them:
http://www.wdtb.noaa.gov/courses/dualpol/Outreach/.

The basic premise behind polarimetric radar is that in addition to
reflectivity estimates that we are familiar with, it estimates the
shapes of hydrometeors. This is accomplished by using both a
horizontally and a vertically polarized radar beam. By measuring the
different returns from these two polarizations, one can estimate the
shape and the effects from different hydrometeor shapes.

For example, we can determine if the prominent reflectors are large
raindrops, which tend to be oblate with a large horizontal axis. We can
also determine if the hydrometeors are more spherical, consistent with
small raindrops. Or we can measure if the hydrometeors are highly
reflective and generally spherical, consistent with hail. Other measures
can be used to estimate the presence of snow, insects, or ground
targets.

|Reflector shape is a function of its size, phase, and type|

**II. Remote Sensing of QPE » Radar Sampling of Precipitation**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Most of the discussion so far is applicable for areas with good radar
coverage. Good radar coverage is determined by three main factors:

1. There are no obstructions of the low-level radar beam from terrain
   features or other ground targets like buildings.

2. Precipitation systems extend through a deep portion of the
   troposphere, as we see with convective storms.

3. The density of radar sites is sufficient. In other words, the radars
   are close enough to each other so that all radar sampling is
   occurring in the low levels of the atmosphere.

|Influences on radar coverage - mountains|

|Influences on radar coverge - deep convection|

|Influences on radar coverage - low level sampling|

The radar beam gets higher in the atmosphere with distance from the
radar. Even a low tilt angle like 0.5° is ~1.5 km (5,000 ft) above the
ground at 100 km from the radar, and 5.2 km (17,000 ft) high at 230 km.
Therefore, to sample the low-level precipitation, which is most likely
to be representative of the precipitation reaching the ground, radars
need to be close to each other.

|Height above the ground of radar sample as a function of range|

For stratiform precipitation it is best to sample the lowest 1 km of the
atmosphere, which typically occurs within 50 km of the radar. Beyond 50
km the radar sample may be questionable. This range can be limited
further by terrain blocking of the radar beam. Sampling of stratiform
precipitation is almost always poor beyond 100 km from the radar.

|Radar coverage of precipitation with range - assuming no beam blocking|

Convective precipitation is distributed over a much deeper layer of the
atmosphere than stratiform precipitation. Therefore, in seasons and
locations where convection is common and terrain is minimal, the radar
may be able to sample precipitation well at long distance from the
radar, perhaps beyond 150 km. Shallow convection may be undersampled by
the radar at closer ranges than 150 km. Range coverage is worse for
snow.

**II. Remote Sensing of QPE » Radar Coverage**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Here are the NWS radar locations with the ideal 230-km range shown with
yellow circles. The density of weather radars is generally lower in the
western United States and Alaska than in other parts of the country.
These maps do not account for terrain features that can greatly reduce
the radar coverage.

|Locations of WSR-88D radars with the idealized 230-km coverge areas|

For many locations and precipitation regimes, it’s unrealistic to expect
good precipitation estimates with the ideal 230-km coverage shown here.
A more realistic radius of 100 or 150-km would show bigger and more
numerous gaps, especially in the Western United States. In the winter,
the range of realistic coverage may shrink to less than a 100 km radius.

A more realistic coverage is shown here with a map of the height above
ground level (AGL) of the radar sampling. It is for November 10th, 2008.
Although this map can change depending on weather conditions and radar
operations, the basic pattern will be the same.

|Height above ground level of radar coverage, 1755 UTC 10 Nov 2008
CONUS|

The light blues show where there is good coverage of the low levels. The
best low level coverage is obviously in areas with relatively flat
terrain and good radar density. Recall that for stratiform
precipitation, radar coverage can be significantly impacted if the radar
sampling is 1 km or more above the ground, as shown in the dark blue,
greens, yellows, and reds. Even in the central and eastern U.S.,
stratiform precipitation may be significantly underestimated in places.
In the West, radar sampling can be more than 3 km above the ground in
large areas. This results in completely missing precipitation systems,
especially stratiform. This is also a problem in Alaska. As an example
let’s look more closely at radar coverage in the northwestern portion of
the contiguous United States.

**II. Remote Sensing of QPE » Radar Climatology**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

To account for the geographic and seasonal variability, the NWS has
radar coverage maps. Here we see the warm-season effective radar
coverage for the Northwest. The color-shaded areas are where radar
climatology shows good coverage from at least one radar. The individual
colors depict which radar the “good” coverage will come from. For
example, the white area shows where radar estimates would come from the
radar at Boise, Idaho, KCBX.

|Warm season radar coverage for the northwest river forecast center
area|

KCBX is considered good here because 1) that radar is able to sample
precipitation, and 2) in areas of overlap with neighboring radars, KCBX
is sampling from a lower elevation. The jagged appearance is caused by
mountains preventing uniform good coverage throughout the entire 230-km
radius.

These are produced by the NWS radar climatology program, RADCLIM. We
will briefly demonstrate radar climatology based on frequency of
occurrence of precipitation for Boise, Idaho.

|Radar climatology analysis and display (Radclim)|

The precipitation frequency of occurrence starts with a precipitation
threshold for defining what we will consider precipitation. Let’s use a
threshold of 0.0 mm which means that any time there is more than 0.0 mm
detected by the radar, we have a precipitation event. We could choose a
higher threshold if we want to filter out light events.

The frequency of precipitation, for each radar bin, is the number of
times more than 0.0 mm was observed divided by all of the radar
observations in the data set. We get this image for the Boise radar. The
radar is in the center of the 230-km radius of ideal radar coverage.

|Frequency of occurrence of non-zero radar-derived precipitation at the
Boise, ID (KCBX): Warm season|

The different colors show the different frequencies of occurrence. As
distance increases from the radar the frequency of precipitation
decreases, indicated by blue and black colors. Note the large areas with
very low frequencies of occurrence, seen as black. These do not
represent natural precipitation distribution. Rather, it shows where the
radar sampling is greatly inhibited by terrain blocking.

**II. Remote Sensing of QPE » Radar Coverage Map**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

So now we want to choose a precipitation frequency threshold to
represent effective radar coverage. In other words, we will say, “only
when precipitation occurred at least this often, will we trust the radar
estimates.”

In this example, a frequency of occurrence of 0.006 was chosen. This
means that we will only consider radar bins where greater than 0.0 mm
occurred at least 0.006, or 0.6% of the time according to the radar
climatology.

|Frequency of occurrence of non-zero radar-derived precipitation at the
Boise, ID (KCBX): Warm season|

This is all non-black shaded areas shown on the radar coverage map as
white shading. So the white shading is where we assume good radar
coverage. We should assume bad coverage in the black areas. In the black
areas, precipitation estimates should come from other radars or other
sources such as rain gauges and satellite.

|Warm season effective radar coverage for Boise, ID (KCBX)|

The choice of frequency threshold is somewhat subjective, based on
forecaster experience regarding what produces the most useful guidance.

Radar climatologies are generated for specific months or seasons. Let’s
go back to the summer season radar coverage for the northwestern portion
of the contiguous United States. All of the non-black areas are where we
can assume good radar coverage. Again, here is the Boise coverage area
that we just talked about. So the white shading is where we can assume
good coverage.

In the cool season, there is more low level precipitation and thus the
effects of terrain and distance on radar precipitation estimates are
more severe. Note the sharp decrease in good radar coverage in the radar
coverage map for the Northwest in the cool season.

|image3|

|Cool season radar coverage for the northwest river forecast center|

These types of radar coverage maps, based on radar climatology, are used
in MPE to determine where radar-derived data should be used.

**II. Remote Sensing of QPE » Satellite QPE**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Satellite estimation of precipitation is potentially useful in areas
with poor coverage from radars and rain gauges. Although satellite
sampling is more consistent from place to place than radar sampling,
satellite-derived precipitation is lower resolution and generally less
accurate than radar-derived precipitation. It is therefore considered a
supplement, not a replacement for the radar products.

|1 hr satellite estimated precip as of 1515 UTC 17 Apr 2009|

Satellite-derived rainfall products perform best in the tropics and in
the middle latitudes during the warm season. In other words it verifies
best when the wind shear is relatively low and precipitation is
dominated by convection. These are not the conditions in the
radar-sparse western United States during the wintertime wet season.

This NOAA product known as the hydro-estimator applies a terrain factor
to the precipitation estimate using 700 mb winds. This helps with
resolving the spatial distribution of the precipitation. Other
improvements to precipitation rates may be achieved by applying factors
related to cloud, moisture, and stability characteristics.

|24 hr satellite estimated precip as of 1200 UTC 5 Jan 2008|

For satellite Hydro-Estimator rainfall products:
http://www.star.nesdis.noaa.gov/smcd/emb/ff/HydroEst.php

In addition to adjustments based on both measured and modeled
environmental properties, there is increasing use of additional sensor
capabilities such as microwave satellite sensing and lightning
detection. Passive microwave observations allow detection of water and
ice within the cloud for derivation of more accurate rainfall rates.
However, because microwave sensing capabilities are specific to
polar-orbiting satellites, the temporal frequency is much less than that
of the hydro-estimator products based on geostationary satellites.

The SCaMPR product, (which stands for Self-Calibrating Multivariate
Precipitation Retrieval) is an example of combining the temporal
resolution of geostationary satellites with the more accurate estimation
of rainfall rates of polar orbiters, and previews the next generation of
operational satellite-based precipitation estimation tools.

|SCaMPR 24 hr estimated precip at 1200 UTC 13 Apr 2009|

For more information on efforts pertaining to real time satellite-based
precipitation estimation at NOAA, please see:
http://www.star.nesdis.noaa.gov/smcd/emb/ff/index.html.

Multi-satellite precipitation products have also greatly benefited from
the new constellation of polar-orbiting satellites, known as the GPM, or
Global Precipitation Measurement mission.

**II. Remote Sensing of QPE » Remote Sensing QPE Key Points**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

-  Radar data, where available, provide the best resolution in space and
   time.

-  The best radar coverage occurs with convective precipitation, liquid
   precipitation, and in regions with minimal terrain features.

-  Errors in radar-derived precipitation are associated with variations
   in drop size distributions, precipitation phase, and lack of
   low-level information.

-  Dual-polarized radars estimate hydrometeor shapes, and should assist
   with developing more accurate precipitation products.

-  Satellite-derived precipitation is a supplement in regions with poor
   radar and rain gauge coverage.

.. |24h QPE| image:: media/ch3/image_obs_popout_radarqpe16.jpg
   :width: 6.04167in
   :height: 4.58333in
.. |48 h QPE| image:: media/ch3/image_obs_popout_radarqpe35.jpg
   :width: 6.04167in
   :height: 4.58333in
.. |Illustration of radar, satellite and rain gauges sensing a convective cloud system.| image:: media/ch3/image_obs_popout_radarqpe13.jpg
   :width: 6.02778in
   :height: 4.125in
.. |image1| image:: media/ch3/image_obs_popout_radarqpe21.jpg
   :width: 6.02778in
   :height: 4.125in
.. |image2| image:: media/ch3/image_obs_popout_radarqpe34.jpg
   :width: 6.02778in
   :height: 4.125in
.. |Radar-derived Total Accumulation| image:: media/ch3/image_obs_popout_radarqpe36.jpg
   :width: 5in
   :height: 6.04167in
.. |Hybrid Reflectivity near LaCrosse, WS 0057 UTC 19 Aug 2007| image:: media/ch3/image_obs_popout_radarqpe28.jpg
   :width: 6.04167in
   :height: 5in
.. |Instantaneous Radar-derived Rainfall Rate near LaCrosse, WS at 0057 UTC 19 Aug 2007| image:: media/ch3/image_obs_popout_radarqpe26.jpg
   :width: 6.04167in
   :height: 5in
.. |Storm Total Radar-Derived Rainfall Accumulation near LaCrosse, WS 0057 UTC 19 Aug 2007| image:: media/ch3/image_obs_popout_radarqpe8.jpg
   :width: 6.04167in
   :height: 5in
.. |Convective storm illustration with close up of hydrometeor sizes| image:: media/ch3/image_obs_popout_radarqpe31.jpg
   :width: 6.02778in
   :height: 4.15278in
.. |Convective storm illustration with close up of hydrometeor concentration| image:: media/ch3/image_obs_popout_radarqpe30.jpg
   :width: 6.02778in
   :height: 4.15278in
.. |Convective storm illustration with close up of hydrometeor phases| image:: media/ch3/image_obs_popout_radarqpe6.jpg
   :width: 6.02778in
   :height: 4.15278in
.. |Convective storm illustration with close up of non-hydrometeors| image:: media/ch3/image_obs_popout_radarqpe18.jpg
   :width: 6.02778in
   :height: 4.15278in
.. |Convective storm illustration with hydrometeor sampling by radar| image:: media/ch3/image_obs_popout_radarqpe11.jpg
   :width: 6.02778in
   :height: 4.15278in
.. |Drop shapes as a function of size| image:: media/ch3/image_obs_popout_radarqpe32.jpg
   :width: 6.04167in
   :height: 4.16667in
.. |DSDs with equivalent reflectivity but different rainfall rates| image:: media/ch3/image_obs_popout_radarqpe10.jpg
   :width: 6.04167in
   :height: 4.16667in
.. |Reflectivity Image at 2126 UTC 15 November 2008| image:: media/ch3/image_obs_popout_radarqpe9.jpg
   :width: 6.04167in
   :height: 5in
.. |Radar and melting snow| image:: media/ch3/image_obs_popout_radarqpe17.jpg
   :width: 5.51389in
   :height: 4.44444in
.. |Sample data from dual-polarimetric Radar| image:: media/ch3/image_obs_popout_radarqpe3.jpg
   :width: 6.04167in
   :height: 4.69444in
.. |Reflector shape is a function of its size, phase, and type| image:: media/ch3/image_obs_popout_radarqpe4.jpg
   :width: 6.04167in
   :height: 4.16667in
.. |Influences on radar coverage - mountains| image:: media/ch3/image_obs_popout_radarqpe29.jpg
   :width: 6.05556in
   :height: 4.13889in
.. |Influences on radar coverge - deep convection| image:: media/ch3/image_obs_popout_radarqpe5.jpg
   :width: 6.05556in
   :height: 4.13889in
.. |Influences on radar coverage - low level sampling| image:: media/ch3/image_obs_popout_radarqpe2.jpg
   :width: 6.05556in
   :height: 4.13889in
.. |Height above the ground of radar sample as a function of range| image:: media/ch3/image_obs_popout_radarqpe22.jpg
   :width: 6.04167in
   :height: 4.16667in
.. |Radar coverage of precipitation with range - assuming no beam blocking| image:: media/ch3/image_obs_popout_radarqpe7.jpg
   :width: 6.04167in
   :height: 4.15278in
.. |Locations of WSR-88D radars with the idealized 230-km coverge areas| image:: media/ch3/image_obs_popout_radarqpe37.jpg
   :width: 6.04167in
   :height: 4.69444in
.. |Height above ground level of radar coverage, 1755 UTC 10 Nov 2008 CONUS| image:: media/ch3/image_obs_popout_radarqpe1.jpg
   :width: 6.04167in
   :height: 4.16667in
.. |Warm season radar coverage for the northwest river forecast center area| image:: media/ch3/image_obs_popout_radarqpe15.jpg
   :width: 6.04167in
   :height: 4.16667in
.. |Radar climatology analysis and display (Radclim)| image:: media/ch3/image_obs_popout_radarqpe14.jpg
   :width: 6.04167in
   :height: 5.09722in
.. |Frequency of occurrence of non-zero radar-derived precipitation at the Boise, ID (KCBX): Warm season| image:: media/ch3/image_obs_popout_radarqpe20.jpg
   :width: 6.04167in
   :height: 4.16667in
.. |Warm season effective radar coverage for Boise, ID (KCBX)| image:: media/ch3/image_obs_popout_radarqpe33.jpg
   :width: 6.04167in
   :height: 4.16667in
.. |image3| image:: media/ch3/image_obs_popout_radarqpe19.jpg
   :width: 6.04167in
   :height: 4.16667in
.. |Cool season radar coverage for the northwest river forecast center| image:: media/ch3/image_obs_popout_radarqpe12.jpg
   :width: 6.04167in
   :height: 4.16667in
.. |1 hr satellite estimated precip as of 1515 UTC 17 Apr 2009| image:: media/ch3/image_obs_popout_radarqpe25.jpg
   :width: 6.04167in
   :height: 4.58333in
.. |24 hr satellite estimated precip as of 1200 UTC 5 Jan 2008| image:: media/ch3/image_obs_popout_radarqpe24.jpg
   :width: 6.04167in
   :height: 4.58333in
.. |SCaMPR 24 hr estimated precip at 1200 UTC 13 Apr 2009| image:: media/ch3/image_obs_popout_radarqpe23.jpg
   :width: 6.04167in
   :height: 4.58333in
