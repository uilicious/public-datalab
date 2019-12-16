```
Testing: e2-standard-4
Running 1m test @ http://10.128.0.6
  16 threads and 500 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency    52.66ms  147.16ms   1.99s    90.00%
    Req/Sec     2.96k     1.81k   25.50k    69.97%
  Latency Distribution
     50%  213.00us
     75%  590.00us
     90%  199.84ms
     99%  694.36ms
  2708642 requests in 1.00m, 2.14GB read
  Socket errors: connect 0, read 110, write 0, timeout 159
Requests/sec:  45068.98
Transfer/sec:     36.53MB

Testing: n1-standard-4
Running 1m test @ http://10.128.0.7
  16 threads and 500 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency    27.86ms   87.13ms   1.84s    91.19%
    Req/Sec     5.12k     2.91k   23.22k    65.93%
  Latency Distribution
     50%  223.00us
     75%  411.00us
     90%  105.39ms
     99%  356.74ms
  4793644 requests in 1.00m, 3.79GB read
  Socket errors: connect 0, read 30, write 0, timeout 66
Requests/sec:  79791.44
Transfer/sec:     64.68MB

Testing: n2-standard-4
Running 1m test @ http://10.128.0.8
  16 threads and 500 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency    29.31ms   99.63ms   1.83s    94.25%
    Req/Sec     5.81k     2.82k   26.52k    68.68%
  Latency Distribution
     50%  209.00us
     75%  812.00us
     90%   98.46ms
     99%  432.24ms
  5430897 requests in 1.00m, 4.30GB read
  Socket errors: connect 0, read 3, write 0, timeout 87
Requests/sec:  90388.18
Transfer/sec:     73.27MB
```