
BenchmarkDotNet=v0.13.2, OS=Windows 11 (10.0.22000.1335/21H2)
AMD Ryzen 3 5300U with Radeon Graphics, 1 CPU, 8 logical and 4 physical cores
.NET SDK=7.0.101
  [Host]     : .NET 6.0.11 (6.0.1122.52304), X64 RyuJIT AVX2 DEBUG
  Job-RNPGDU : .NET 6.0.11 (6.0.1122.52304), X64 RyuJIT AVX2

InvocationCount=1  UnrollFactor=1  

                  Method | insertTimes |      Mean |     Error |    StdDev |    Median | Allocated |
------------------------ |------------ |----------:|----------:|----------:|----------:|----------:|
  **DeleteFromStartOfTable** |         **100** |  **1.803 μs** | **0.0391 μs** | **0.0654 μs** |  **1.800 μs** |     **648 B** |
   DeleteFromStartOfRope |         100 |  5.200 μs | 0.0766 μs | 0.0679 μs |  5.200 μs |     880 B |
 DeleteFromMiddleOfTable |         100 |  2.353 μs | 0.0963 μs | 0.2652 μs |  2.300 μs |     688 B |
  DeleteFromMiddleOfRope |         100 |  5.340 μs | 0.1101 μs | 0.2013 μs |  5.300 μs |     880 B |
    DeleteFromEndOfTable |         100 |  1.910 μs | 0.0408 μs | 0.0735 μs |  1.900 μs |     688 B |
     DeleteFromEndOfRope |         100 |  5.027 μs | 0.0489 μs | 0.0458 μs |  5.000 μs |     872 B |
  **DeleteFromStartOfTable** |        **1000** |  **3.328 μs** | **0.4499 μs** | **1.2909 μs** |  **2.800 μs** |     **648 B** |
   DeleteFromStartOfRope |        1000 |  6.740 μs | 0.2379 μs | 0.6514 μs |  6.500 μs |    1000 B |
 DeleteFromMiddleOfTable |        1000 |  3.619 μs | 0.4529 μs | 1.3141 μs |  3.000 μs |     688 B |
  DeleteFromMiddleOfRope |        1000 |  9.304 μs | 1.2926 μs | 3.7910 μs |  7.900 μs |    1000 B |
    DeleteFromEndOfTable |        1000 |  2.685 μs | 0.1712 μs | 0.4883 μs |  2.500 μs |     688 B |
     DeleteFromEndOfRope |        1000 |  8.528 μs | 1.1650 μs | 3.3797 μs |  6.700 μs |     992 B |
  **DeleteFromStartOfTable** |       **10000** |  **5.701 μs** | **0.6786 μs** | **1.9902 μs** |  **5.700 μs** |     **648 B** |
   DeleteFromStartOfRope |       10000 | 12.799 μs | 0.6320 μs | 1.7723 μs | 12.100 μs |    1160 B |
 DeleteFromMiddleOfTable |       10000 |  5.428 μs | 0.6586 μs | 1.9003 μs |  5.000 μs |     688 B |
  DeleteFromMiddleOfRope |       10000 | 12.933 μs | 0.5333 μs | 1.5302 μs | 12.800 μs |    1160 B |
    DeleteFromEndOfTable |       10000 |  5.936 μs | 0.6513 μs | 1.8999 μs |  5.950 μs |     688 B |
     DeleteFromEndOfRope |       10000 | 12.994 μs | 0.3403 μs | 0.9373 μs | 12.800 μs |    1152 B |
