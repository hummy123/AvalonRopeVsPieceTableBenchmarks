
BenchmarkDotNet=v0.13.2, OS=Windows 11 (10.0.22000.1335/21H2)
AMD Ryzen 3 5300U with Radeon Graphics, 1 CPU, 8 logical and 4 physical cores
.NET SDK=7.0.101
  [Host]     : .NET 6.0.11 (6.0.1122.52304), X64 RyuJIT AVX2 DEBUG
  Job-YMQLEL : .NET 6.0.11 (6.0.1122.52304), X64 RyuJIT AVX2

InvocationCount=1  UnrollFactor=1  

                 Method | insertTimes |         Mean |       Error |     StdDev |       Median | Allocated |
----------------------- |------------ |-------------:|------------:|-----------:|-------------:|----------:|
  **GetCharAtStartOfTable** |         **100** |   **1,614.6 ns** |    **44.39 ns** |   **117.7 ns** |   **1,600.0 ns** |     **504 B** |
   GetCharAtStartOfRope |         100 |   2,213.4 ns |   253.52 ns |   735.5 ns |   2,100.0 ns |     520 B |
 GetCharAtMiddleOfTable |         100 |   7,008.6 ns |   514.40 ns | 1,459.3 ns |   6,700.0 ns |    4176 B |
  GetCharAtMiddleOfRope |         100 |     508.7 ns |    90.83 ns |   256.2 ns |     400.0 ns |     480 B |
    GetCharAtEndOfTable |         100 |   8,213.0 ns |   361.57 ns | 1,019.8 ns |   8,050.0 ns |    7416 B |
     GetCharAtEndOfRope |         100 |           NA |          NA |         NA |           NA |         - |
  **GetCharAtStartOfTable** |        **1000** |   **5,433.3 ns** |   **551.03 ns** | **1,563.2 ns** |   **5,200.0 ns** |     **504 B** |
   GetCharAtStartOfRope |        1000 |   2,922.9 ns |   354.37 ns | 1,022.4 ns |   2,550.0 ns |     680 B |
 GetCharAtMiddleOfTable |        1000 |  28,174.7 ns | 2,012.94 ns | 5,644.5 ns |  30,100.0 ns |   36576 B |
  GetCharAtMiddleOfRope |        1000 |   2,031.2 ns |   245.27 ns |   695.8 ns |   1,700.0 ns |     304 B |
    GetCharAtEndOfTable |        1000 |  51,338.5 ns |   742.31 ns |   619.9 ns |  51,200.0 ns |   72552 B |
     GetCharAtEndOfRope |        1000 |           NA |          NA |         NA |           NA |         - |
  **GetCharAtStartOfTable** |       **10000** |   **4,646.3 ns** |   **612.64 ns** | **1,757.8 ns** |   **3,700.0 ns** |     **504 B** |
   GetCharAtStartOfRope |       10000 |   2,339.1 ns |   172.09 ns |   485.4 ns |   2,200.0 ns |     800 B |
 GetCharAtMiddleOfTable |       10000 | 121,925.0 ns | 1,299.49 ns | 1,014.6 ns | 121,900.0 ns |  360576 B |
  GetCharAtMiddleOfRope |       10000 |   2,852.1 ns |   389.62 ns | 1,111.6 ns |   2,350.0 ns |     760 B |
    GetCharAtEndOfTable |       10000 | 244,098.0 ns | 4,389.95 ns | 8,967.5 ns | 241,700.0 ns |  720552 B |
     GetCharAtEndOfRope |       10000 |           NA |          NA |         NA |           NA |         - |

Benchmarks with issues:
  GetCharAtIndex.GetCharAtEndOfRope: Job-YMQLEL(InvocationCount=1, UnrollFactor=1) [insertTimes=100]
  GetCharAtIndex.GetCharAtEndOfRope: Job-YMQLEL(InvocationCount=1, UnrollFactor=1) [insertTimes=1000]
  GetCharAtIndex.GetCharAtEndOfRope: Job-YMQLEL(InvocationCount=1, UnrollFactor=1) [insertTimes=10000]
