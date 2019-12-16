```
eugene@e2-standard-4:~$ sysbench --test=memory --num-threads=4 run
sysbench 0.4.12:  multi-threaded system evaluation benchmark
Running the test with following options:
Number of threads: 4
Doing memory operations speed test
Memory block size: 1K
Memory transfer size: 102400M
Memory operations type: write
Memory scope type: global
Threads started!
Done.
Operations performed: 104857600 (4239992.37 ops/sec)
102400.00 MB transferred (4140.62 MB/sec)
Test execution summary:
    total time:                          24.7306s
    total number of events:              104857600
    total time taken by event execution: 73.5318
    per-request statistics:
         min:                                  0.00ms
         avg:                                  0.00ms
         max:                                 24.01ms
         approx.  95 percentile:               0.00ms
Threads fairness:
    events (avg/stddev):           26214400.0000/135310.12
    execution time (avg/stddev):   18.3830/0.15

eugene@n1-standard-4:~$ sysbench --test=memory --num-threads=4 run
sysbench 0.4.12:  multi-threaded system evaluation benchmark
Running the test with following options:
Number of threads: 4
Doing memory operations speed test
Memory block size: 1K
Memory transfer size: 102400M
Memory operations type: write
Memory scope type: global
Threads started!
Done.
Operations performed: 104857600 (2440138.74 ops/sec)
102400.00 MB transferred (2382.95 MB/sec)
Test execution summary:
    total time:                          42.9720s
    total number of events:              104857600
    total time taken by event execution: 106.8365
    per-request statistics:
         min:                                  0.00ms
         avg:                                  0.00ms
         max:                                  2.96ms
         approx.  95 percentile:               0.00ms
Threads fairness:
    events (avg/stddev):           26214400.0000/523071.94
    execution time (avg/stddev):   26.7091/0.22

eugene@n2-standard-4:~$ sysbench --test=memory --num-threads=4 run
sysbench 0.4.12:  multi-threaded system evaluation benchmark

Running the test with following options:
Number of threads: 4

Doing memory operations speed test
Memory block size: 1K

Memory transfer size: 102400M

Memory operations type: write
Memory scope type: global
Threads started!
Done.

Operations performed: 104857600 (2596116.93 ops/sec)

102400.00 MB transferred (2535.27 MB/sec)


Test execution summary:
    total time:                          40.3902s
    total number of events:              104857600
    total time taken by event execution: 97.5529
    per-request statistics:
         min:                                  0.00ms
         avg:                                  0.00ms
         max:                                  3.27ms
         approx.  95 percentile:               0.00ms

Threads fairness:
    events (avg/stddev):           26214400.0000/325686.94
    execution time (avg/stddev):   24.3882/0.06
```