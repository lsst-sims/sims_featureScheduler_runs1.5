# sims_featureScheduler_runs1.5
v1.5 of simulations of the LSST scheduler

XXX--not final yet, will be anounced on community.lsst.org when released

We run a few isolated experiemnts, and then generate a few tuned and customized results that can be seen as starting points for a final scheduler.

## dcr

An experiemnt looking at intentionally taking some observations at high airmass to help with DCR model construction as well as science enabled by measuring the DCR of objects.

## filter_dist

Looking at different filter distributions.

## potential_scedulers

For most, try to tune so we get around 875-900 visits in the WFD area. 

### Bare Bones

This is an intentionally "bad" simulation, where we only strive to meet the SRD requirements, but have not particularly crafted a useful strategy for science. This is a good example of just how deep the WFD area could possibly get.

Only WFD area, minimal DDF cadence. pairs in same filter.

This could be considered the "emergency strategy to meet SRD", e.g., we reach year 8 or 9 of the survey and project we will fall short of the SRD requirements, a strategy like this could be used to make sure we reach SRD values.

Plusses: 

* This meets SRD

Minuses: 

* No NES, so Solar System should suffer
* No color info on pairs, so transients will suffer
* No Galactic plane coverage, so no bulge science, and hard to ubercal the survey


### Classic Baseline

The lastest iteration of our baseline survey. With 1 and 2 snaps per visit.

### Rolling Exgal

Use a footprint that de-emphasizes the dusty plane of the galaxy. Use a rolling cadence strategy on the WFD area to generate more densly sampled light curves. Standard DDF strategy.

Should this include good seeing images?

### DM Heavy
A simulation that is inspired by DM considerations

* large dithers for DDF fields
* rotator angle set to align spiders along rows and columns
* Get DCR images in ugr
* g,r,i images of the whole sky in good seeing 

##3 MW local group heavy

Cover the bulge, galactic anti-center and LMC/SMC in depth.

### DDF heavy

Give as much time as possible to the DDF surveys.  Looks like it might have hit the limit of what they can do running once per day? Can make sequences longer and/or extend seasons.

### Solar System Heavy

Slap extra gri all over the ecliptic maybe?   NEO survey at twilight.
