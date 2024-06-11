.. vim: syntax=rst

**IV. Precipitation Climatology/PRISM**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Precipitation climatology guidance can be used to help fill in the gaps
where estimates of observed precipitation are poor. The most widely used
precipitation climatology tool in the United States as of 2009 is the
Parameter-elevation Regressions on an Independent Slopes Model, or
PRISM. Prior to its use in multiple-sensor precipitation estimation
(MPE), PRISM was used extensively in several River Forecast Centers in
the western United States.

|Prism precipitation maps|

Topics in this section include the rationale for PRISM, the use of PRISM
data, and limitations of using precipitation climatology for QPE.

**IV. Precipitation Climatology/PRISM » PRISM**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Developed at Oregon State University, PRISM climatology products include
precipitation climatology guidance for the contiguous United States...

|PRISM precipitation: annual climatology for the CONUS 1971-2000|

...the Hawaiian Islands, Puerto Rico, Guam, and...

|PRISM Precipitation annual climatology for Hawaii|

...Alaska, along with portions of neighboring Canadian provinces.

|PRISM Precipitation Annual climatology for Alaska and the Yukon|

Products and detailed presentations about deriving those products are
available for download from the PRISM group at Oregon State University:
http://www.prism.oregonstate.edu/.

PRISM precipitation climatologies are based on the historic record of
measured precipitation at point locations, geographic input, especially
terrain information, and in some cases, the prevailing wind direction.
Streamflow discharge measurements are used to correlate basin
precipitation climatology with runoff climatology and thus provide a
rough validation check on the precipitation amount.

|Gauge locations and topography of Olympic peninsula|

Point observations are rarely sufficient to represent spatial patterns
of precipitation. This is especially true in regions with sharp changes
in elevation and/or nearby large bodies of water. PRISM uses the known
relationships of precipitation with geographic features. An automated
statistical approach is used for efficiency, but this is guided by human
expertise.

|PRISM annual precip climatology with rain gauge locations for the
Olympic peninsula|

**IV. Precipitation Climatology/PRISM » Basic Use of PRISM**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

PRISM precipitation climatology may be used for both observed
precipitation (QPE) and forecast precipitation (QPF).

Deriving QPE from PRISM precipitation climatology starts with point
values, such as reading from a rain gauge. From there we derive the
ratio of the point value to the PRISM value.

|Using gauge reports and PRISM to get QPE 2|

In this example we assume the gauge reading is 40 mm (1.57 in) and the
PRISM value at that point is 20 mm (0.79 in). The ratio of 40 over 20 is
2.0. Now, we apply that ratio to other PRISM values.

|Using gauge reports and PRISM to get QPE 3|

This adjusts the areal precipitation estimate by the ratio of 2.0 but it
preserves the gradients and the relative magnitudes that we see in the
PRISM data.

|Using gauge reports and PRISM to get QPE 4|

Of course this process is done for numerous gauge locations using
distance-weighting schemes.

|24-hr precip accumulation from daily QC program as of 1200 UTC 23 Jan
2008|

This approach using gauge and terrain data is considered the
3-dimensional (3-D) approach. This can be very useful in
terrain-affected areas. The areas that are within 100 km of the green
shading on this map are where PRISM uses the 3-D approach for QPE. This
would also include all of the Hawaiian Islands and most of Alaska. In
the white areas on this map, PRISM uses a 2-D process. This is basically
a distance-weighted gauge analysis.

|PRISM effective terrain areas|

**IV. Precipitation Climatology/PRISM » Limitations of Precipitation Climatology**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

As with any climatological data, there are limitations. Climatology
averages the individual events in a data set. Individual precipitation
events may show large departures from climatology, especially in the
locations of extreme and sharp gradients. However, even with these
limitations, there are regions that will likely benefit somewhat from
climatological tools.

Individual events will often be closer to climatology in regions with
large orographic influences.

|Salt lake city|

In addition, regions that tend to receive widespread, stratiform
precipitation will be closer to climatology than areas dominated by
convection.

|Strat clounds rainy road with cars|

So the western coasts of North America may be the areas that can benefit
most from climatological adjustments to QPE. Keep in mind that
departures from climatological norms will likely have greater impacts as
one looks at smaller basins.

.. |Prism precipitation maps| image:: media/ch3/image_obs_popout_prism11.jpg
   :width: 4.48611in
   :height: 3.65278in
.. |PRISM precipitation: annual climatology for the CONUS 1971-2000| image:: media/ch3/image_obs_popout_prism1.jpg
   :width: 6.04167in
   :height: 4.58333in
.. |PRISM Precipitation annual climatology for Hawaii| image:: media/ch3/image_obs_popout_prism9.jpg
   :width: 6.04167in
   :height: 4.58333in
.. |PRISM Precipitation Annual climatology for Alaska and the Yukon| image:: media/ch3/image_obs_popout_prism12.jpg
   :width: 6.04167in
   :height: 4.58333in
.. |Gauge locations and topography of Olympic peninsula| image:: media/ch3/image_obs_popout_prism13.jpg
   :width: 6.04167in
   :height: 4.55556in
.. |PRISM annual precip climatology with rain gauge locations for the Olympic peninsula| image:: media/ch3/image_obs_popout_prism3.jpg
   :width: 6.04167in
   :height: 4.79167in
.. |Using gauge reports and PRISM to get QPE 2| image:: media/ch3/image_obs_popout_prism5.jpg
   :width: 5.18056in
   :height: 4.52778in
.. |Using gauge reports and PRISM to get QPE 3| image:: media/ch3/image_obs_popout_prism10.jpg
   :width: 5.27778in
   :height: 4.51389in
.. |Using gauge reports and PRISM to get QPE 4| image:: media/ch3/image_obs_popout_prism2.jpg
   :width: 5.09722in
   :height: 4.51389in
.. |24-hr precip accumulation from daily QC program as of 1200 UTC 23 Jan 2008| image:: media/ch3/image_obs_popout_prism8.jpg
   :width: 6.04167in
   :height: 5in
.. |PRISM effective terrain areas| image:: media/ch3/image_obs_popout_prism6.jpg
   :width: 6.04167in
   :height: 4.16667in
.. |Salt lake city| image:: media/ch3/image_obs_popout_prism4.jpg
   :width: 6.25in
   :height: 4.15278in
.. |Strat clounds rainy road with cars| image:: media/ch3/image_obs_popout_prism7.jpg
   :width: 5.73611in
   :height: 4.13889in
