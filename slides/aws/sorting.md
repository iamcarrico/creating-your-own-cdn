## Sorting

Note:
Route 53 allows for latency-based DNS routing. Simply put: it sorts traffic to the server closet to them (based on latency). There is a slight downside, which is that it is based off the locations of Amazon's datacenters— not necessarily where your servers are. Luckily, my servers were in the same city as where Amazon's server farms are thus making this work very well.
