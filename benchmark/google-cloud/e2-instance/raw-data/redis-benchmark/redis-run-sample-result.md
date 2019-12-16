```
eugene@e2-standard-4:~$ time redis-benchmark -q 
PING_INLINE: 90826.52 requests per second
PING_BULK: 81168.83 requests per second
SET: 85178.88 requests per second
GET: 85763.29 requests per second
INCR: 88417.33 requests per second
LPUSH: 90497.73 requests per second
RPUSH: 86206.90 requests per second
LPOP: 89445.44 requests per second
RPOP: 88809.95 requests per second
SADD: 89126.56 requests per second
SPOP: 88417.33 requests per second
LPUSH (needed to benchmark LRANGE): 83333.33 requests per second
LRANGE_100 (first 100 elements): 35932.45 requests per second
LRANGE_300 (first 300 elements): 12241.40 requests per second
LRANGE_500 (first 450 elements): 8232.49 requests per second
LRANGE_600 (first 600 elements): 6428.39 requests per second
MSET (10 keys): 67340.07 requests per second
real    0m53.930s
user    0m37.280s
sys     0m16.148s

eugene@n1-standard-4:~$ time redis-benchmark -q 
PING_INLINE: 101112.23 requests per second
PING_BULK: 99403.58 requests per second
SET: 102354.15 requests per second
GET: 99206.34 requests per second
INCR: 102354.15 requests per second
LPUSH: 102774.92 requests per second
RPUSH: 103519.66 requests per second
LPOP: 100908.17 requests per second
RPOP: 102880.66 requests per second
SADD: 102354.15 requests per second
SPOP: 102880.66 requests per second
LPUSH (needed to benchmark LRANGE): 102354.15 requests per second
LRANGE_100 (first 100 elements): 48053.82 requests per second
LRANGE_300 (first 300 elements): 21772.26 requests per second
LRANGE_500 (first 450 elements): 14336.92 requests per second
LRANGE_600 (first 600 elements): 11147.03 requests per second
MSET (10 keys): 79744.82 requests per second
real    0m35.676s
user    0m21.796s
sys     0m13.140s

eugene@n2-standard-4:~$ time redis-benchmark -q 
PING_INLINE: 112739.57 requests per second
PING_BULK: 109051.26 requests per second
SET: 111111.12 requests per second
GET: 112107.62 requests per second
INCR: 110011.00 requests per second
LPUSH: 112866.82 requests per second
RPUSH: 114942.53 requests per second
LPOP: 113765.64 requests per second
RPOP: 112994.35 requests per second
SADD: 112739.57 requests per second
SPOP: 109051.26 requests per second
LPUSH (needed to benchmark LRANGE): 116959.06 requests per second
LRANGE_100 (first 100 elements): 62500.00 requests per second
LRANGE_300 (first 300 elements): 24857.07 requests per second
LRANGE_500 (first 450 elements): 16949.15 requests per second
LRANGE_600 (first 600 elements): 13095.86 requests per second
MSET (10 keys): 117233.30 requests per second
real    0m30.712s
user    0m18.408s
sys     0m12.216s
```