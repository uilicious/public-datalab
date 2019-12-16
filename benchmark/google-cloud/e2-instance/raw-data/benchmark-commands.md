# install commands

```
sudo apt-get update
sudo apt-get install -y sysbench 
```

# sysbench

```
sysbench --test=cpu --cpu-max-prime=50000 --num-threads=4 run

sysbench --test=memory --num-threads=4 run

sysbench --test=cpu --cpu-max-prime=1000 --num-threads=4 run
```

```
sysbench --test=threads --thread-locks=1 --max-time=20s run

sysbench --test=mutex --num-threads=64 run
```

# HTTP benchmarking

```
sudo apt-get install -y nginx
```

```
sudo apt-get install -y wrk
wrk --threads 16 --connections 500 --duration 60s --latency http://localhost
```


```
echo "Testing: e2-standard-4" && wrk --threads 16 --connections 500 --duration 10s --latency http://10.128.0.6
echo "Testing: n1-standard-4" && wrk --threads 16 --connections 500 --duration 10s --latency http://10.128.0.7
echo "Testing: n2-standard-4" && wrk --threads 16 --connections 500 --duration 10s --latency http://10.128.0.8
```


```
echo "Testing: e2-standard-4" && wrk --threads 16 --connections 500 --duration 60s --latency http://10.128.0.6
echo "Testing: n1-standard-4" && wrk --threads 16 --connections 500 --duration 60s --latency http://10.128.0.7
echo "Testing: n2-standard-4" && wrk --threads 16 --connections 500 --duration 60s --latency http://10.128.0.8
```

# redis benchmark

```
sudo apt-get install -y redis-server

time redis-benchmark -q 
```