# GCP E2 instance benchmark

The following benchmarks command and results, was performed in `us-central1-f` region. Using `N1/N2/E2-standard-4` instances. With `N1-standard-4` serving the baseline for comparision.

In addition, a seperate `N2-Standard-16` was deployed to perform the HTTP wrk bench tests agains the 3 respective servers.

A much more detailed analaysis is performed at: < insert blog article here >

# Sysbench Setup

```
sudo apt-get update
sudo apt-get install -y sysbench 
```

# Sysbench CPU test

```
sysbench --test=cpu --cpu-max-prime=50000 --num-threads=4 run
```