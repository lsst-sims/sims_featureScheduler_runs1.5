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



## dcr

An experiemnt looking at intentionally taking some observations at high airmass to help with DCR model construction as well as science enabled by measuring the DCR of objects.

## filter_dist

Looking at different filter distributions.

