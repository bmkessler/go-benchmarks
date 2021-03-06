# Introduction
This directory includes timestamp benchmarks for various different time stamp functions.

# Guarantees
Different time functions have different tradeoffs. 

### Staleness
_TODO_

# Setup
```
Ubuntu Linux
Intel(R) Xeon(R) CPU E5-2670 v2 @ 2.50GHz x 20 Cores (40 Hyperthreaded)
L1 Cache:   320 kB
L2 Cache:  2560 kB
L3 Cache: 25600 kB
Memory: 126 GB
```

# Results
[![results](../results/time.png)](https://github.com/kellabyte/go-benchmarks/raw/master/results/time.png)

### p90
[![results](../results/time_p90.png)](https://github.com/kellabyte/go-benchmarks/raw/master/results/time_p90.png)
### p99
[![results](../results/time_p99.png)](https://github.com/kellabyte/go-benchmarks/raw/master/results/time_p99.png)
### p999
[![results](../results/time_p999.png)](https://github.com/kellabyte/go-benchmarks/raw/master/results/time_p999.png)
### p9999
[![results](../results/time_p9999.png)](https://github.com/kellabyte/go-benchmarks/raw/master/results/time_p9999.png)
### p99999
[![results](../results/time_p99999.png)](https://github.com/kellabyte/go-benchmarks/raw/master/results/time_p99999.png)
### p999999
[![results](../results/time_p99999.png)](https://github.com/kellabyte/go-benchmarks/raw/master/results/time_p99999.png)
### p9999999
[![results](../results/time_p999999.png)](https://github.com/kellabyte/go-benchmarks/raw/master/results/time_p999999.png)

```
make queues

goos: linux
goarch: amd64
pkg: github.com/kellabyte/go-benchmarks/time
BenchmarkNanotime-40    	20000000	        59.4 ns/op	  16.82 MB/s	       0 B/op	       0 allocs/op
BenchmarkHrtime-40      	100000000	        21.4 ns/op	  46.76 MB/s	       0 B/op	       0 allocs/op
PASS
ok  	github.com/kellabyte/go-benchmarks/time	11.010s
```