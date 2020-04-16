# sims_featureScheduler_runs1.5
v1.5 of simulations of the LSST scheduler

XXX--not final yet, will be anounced on community.lsst.org when released

Changes from v1.4

* New defualt DDF behavior, limiting DDFs to about 5% of the total visits
* Regions are selected to be more contiguous, reducing the mean slewtime
* Eliminated extra filter changes in DDFs
* Leaving the u filter mounted in the telescope for longer (until 40% lunar illumination)
* No longer taking u+u pairs (only u+g or u+r)
* Improved calculation of 5-sigma depth for variation between 1 and 2 snap visits
* Set 5th deep drilling field to be a pair of Euclid pointings

## DDFs

DDF strategies, including ones from the AGN and DESC white papers.

## alt_roll_dust

Surveys where the WFD footprint is designed to avoid dusty regions. Includes version with rolling strategy and alt-sched North/South alternating strategy.

## baseline

1 and 2 snap baseline strategies.

## bulge

Covering the Milky Way bulge with different strategies.

## daily_ddf

An initial attempt at having DDF fields observed daily.


## dcr

An experiemnt looking at intentionally taking some observations at high airmass to help with DCR model construction as well as science enabled by measuring the DCR of objects.

## filter_dist

Looking at different filter distributions (e.g., red or blue heavy footprints).

## goodseeing

Ensuring the entire sky has an image taken in good seeing conditions every year.

## rolling

Various rolling cadence surveys.

## short_exp

Covering the whole sky in short exposures.

## spiders

Scheduling the camera rotator angle so that diffraction spikes are always along rows and columns.

## third_obs

Dedicating the end of the night to re-observing areas that have been seen in the night.

## twilight_neo

Using twilight time to look for NEOs.

## u60

Increasing u-band visits to 60s.

## var_exp

Using variable exposure times to make visit depths more uniform.

## wfd_depth

Varying the amount of time in the WFD region.
