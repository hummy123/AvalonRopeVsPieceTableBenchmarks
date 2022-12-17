
BenchmarkDotNet=v0.13.2, OS=Windows 11 (10.0.22000.1335/21H2)
AMD Ryzen 3 5300U with Radeon Graphics, 1 CPU, 8 logical and 4 physical cores
.NET SDK=7.0.101
  [Host]     : .NET 6.0.11 (6.0.1122.52304), X64 RyuJIT AVX2 DEBUG
  Job-RNPGDU : .NET 6.0.11 (6.0.1122.52304), X64 RyuJIT AVX2

InvocationCount=1  UnrollFactor=1  

                  Method | insertTimes |      Mean |     Error |    StdDev |    Median | Allocated |
------------------------ |------------ |----------:|----------:|----------:|----------:|----------:|
  **InsertIntoTableAtStart** |         **100** |  **2.391 μs** | **0.0514 μs** | **0.1212 μs** |  **2.400 μs** |    **1808 B** |
   InsertIntoRopeAtStart |         100 |  4.950 μs | 0.1004 μs | 0.1440 μs |  4.950 μs |     816 B |
 InsertIntoTableAtMiddle |         100 |  2.356 μs | 0.0542 μs | 0.1492 μs |  2.300 μs |    1808 B |
  InsertIntoRopeAtMiddle |         100 |  4.931 μs | 0.1024 μs | 0.0855 μs |  4.900 μs |    1984 B |
    InsertIntoTableAtEnd |         100 |  2.464 μs | 0.0659 μs | 0.1814 μs |  2.400 μs |    1808 B |
     InsertIntoRopeAtEnd |         100 |  5.081 μs | 0.1026 μs | 0.1952 μs |  5.050 μs |    1984 B |
  **InsertIntoTableAtStart** |        **1000** |  **6.351 μs** | **0.6680 μs** | **1.9592 μs** |  **5.800 μs** |    **2728 B** |
   InsertIntoRopeAtStart |        1000 |  6.350 μs | 0.3179 μs | 0.8540 μs |  6.050 μs |     936 B |
 InsertIntoTableAtMiddle |        1000 |  3.154 μs | 0.1667 μs | 0.4479 μs |  3.000 μs |    2728 B |
  InsertIntoRopeAtMiddle |        1000 |  6.930 μs | 0.5868 μs | 1.5964 μs |  6.400 μs |    2104 B |
    InsertIntoTableAtEnd |        1000 |  2.978 μs | 0.1181 μs | 0.3212 μs |  2.900 μs |    2728 B |
     InsertIntoRopeAtEnd |        1000 |  6.083 μs | 0.3997 μs | 1.0807 μs |  5.650 μs |    2104 B |
  **InsertIntoTableAtStart** |       **10000** |  **6.540 μs** | **0.3615 μs** | **1.0195 μs** |  **6.200 μs** |    **2840 B** |
   InsertIntoRopeAtStart |       10000 | 12.414 μs | 0.5838 μs | 1.6465 μs | 11.900 μs |    1096 B |
 InsertIntoTableAtMiddle |       10000 |  6.146 μs | 0.2970 μs | 0.8131 μs |  5.900 μs |    2840 B |
  InsertIntoRopeAtMiddle |       10000 | 14.024 μs | 0.2800 μs | 0.7664 μs | 14.000 μs |    2264 B |
    InsertIntoTableAtEnd |       10000 |  6.625 μs | 0.3926 μs | 1.1008 μs |  6.200 μs |    2840 B |
     InsertIntoRopeAtEnd |       10000 | 12.100 μs | 0.3597 μs | 0.9968 μs | 11.900 μs |    2264 B |
