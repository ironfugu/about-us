### CircleCI NVS

To measure productivity can be hard when it comes to development, but is there a way?  His formula for "Net Value Score" or NVS was based on the number of green and red builds across a company's repos, with the range from -1 to 1, with 1 being the best.  The simple formula is as follows

```
1 - (count (red builds)
    --------------------
    count (green builds)
-------------------------
1 + red mins
    --------
    green mins
```
