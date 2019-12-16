```
eugene@e2-standard-4:~$ sysbench --test=cpu --cpu-max-prime=50000 --num-threads=4 run
sysbench 0.4.12:  multi-threaded system evaluation benchmark
Running the test with following options:
Number of threads: 4
Doing CPU performance benchmark
Threads started!
Done.
Maximum prime number checked in CPU test: 50000
Test execution summary:
    total time:                          45.7569s
    total number of events:              10000
    total time taken by event execution: 182.9897
    per-request statistics:
         min:                                  9.00ms
         avg:                                 18.30ms
         max:                                 30.30ms
         approx.  95 percentile:              25.13ms
Threads fairness:
    events (avg/stddev):           2500.0000/2.35
    execution time (avg/stddev):   45.7474/0.01
```

```
sysbench 0.4.12:  multi-threaded system evaluation benchmark
Running the test with following options:
Number of threads: 4
Doing CPU performance benchmark
Threads started!
Done.
Maximum prime number checked in CPU test: 50000
Test execution summary:
    total time:                          26.9450s
    total number of events:              10000
    total time taken by event execution: 107.7613
    per-request statistics:
         min:                                 10.25ms
         avg:                                 10.78ms
         max:                                 18.54ms
         approx.  95 percentile:              10.98ms
Threads fairness:
    events (avg/stddev):           2500.0000/3.16
    execution time (avg/stddev):   26.9403/0.00
```

```
sysbench 0.4.12:  multi-threaded system evaluation benchmark
Running the test with following options:
Number of threads: 4
Doing CPU performance benchmark
Threads started!
Done.
Maximum prime number checked in CPU test: 50000
Test execution summary:
    total time:                          21.7592s
    total number of events:              10000
    total time taken by event execution: 87.0241
    per-request statistics:
         min:                                  8.10ms
         avg:                                  8.70ms
         max:                                 11.99ms
         approx.  95 percentile:               8.79ms
Threads fairness:
    events (avg/stddev):           2500.0000/0.71
    execution time (avg/stddev):   21.7560/0.00
```