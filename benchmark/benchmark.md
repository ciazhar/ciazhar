# Benchmark

# Spring Cloud Gateway
```bash
Running 30s test @ http://localhost:5628/miscellaneous-service/list/
  12 threads and 400 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency   171.04ms   65.25ms 895.52ms   70.55%
    Req/Sec   190.11     50.52   370.00     72.59%
  68049 requests in 30.10s, 33.50MB read
  Socket errors: connect 0, read 312, write 1, timeout 0
Requests/sec:   2261.11
Transfer/sec:      1.11MB  
```

# GRPC Gateway
```bash
Running 30s test @ http://localhost:8080/list
  12 threads and 400 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency    57.93ms   47.96ms 821.78ms   94.89%
    Req/Sec   402.74    231.65     1.04k    63.14%
  131392 requests in 30.09s, 45.49MB read
  Socket errors: connect 157, read 217, write 0, timeout 0
Requests/sec:   4366.97
Transfer/sec:      1.51MB
```