
BenchmarkDotNet=v0.13.2, OS=Windows 11 (10.0.22000.1335/21H2)
AMD Ryzen 3 5300U with Radeon Graphics, 1 CPU, 8 logical and 4 physical cores
.NET SDK=7.0.101
  [Host]     : .NET 6.0.11 (6.0.1122.52304), X64 RyuJIT AVX2 DEBUG
  Job-RNPGDU : .NET 6.0.11 (6.0.1122.52304), X64 RyuJIT AVX2

InvocationCount=1  UnrollFactor=1  

                      Method | insertTimes |     Mean |     Error |    StdDev |   Median | Allocated |
---------------------------- |------------ |---------:|----------:|----------:|---------:|----------:|
      **InsertIntoTableAtStart** |         **100** | **2.260 μs** | **0.0435 μs** | **0.0954 μs** | **2.200 μs** |    **1712 B** |
     InsertIntoTableAtMiddle |         100 | 2.344 μs | 0.0647 μs | 0.1770 μs | 2.300 μs |    1808 B |
        InsertIntoTableAtEnd |         100 | 2.289 μs | 0.0494 μs | 0.1360 μs | 2.200 μs |    1712 B |
      DeleteFromStartOfTable |         100 | 1.887 μs | 0.0485 μs | 0.1369 μs | 1.900 μs |     648 B |
     DeleteFromMiddleOfTable |         100 | 2.322 μs | 0.1041 μs | 0.2867 μs | 2.300 μs |     688 B |
        DeleteFromEndOfTable |         100 | 1.925 μs | 0.0440 μs | 0.1235 μs | 1.900 μs |     688 B |
  GetSubstringAtStartOfTable |         100 | 1.802 μs | 0.0433 μs | 0.1222 μs | 1.800 μs |     528 B |
 GetSubstringAtMiddleOfTable |         100 | 1.975 μs | 0.0365 μs | 0.0686 μs | 2.000 μs |     600 B |
    GetSubstringAtEndOfTable |         100 | 2.092 μs | 0.0370 μs | 0.0289 μs | 2.100 μs |     592 B |
      **InsertIntoTableAtStart** |        **1000** | **2.546 μs** | **0.0811 μs** | **0.2219 μs** | **2.500 μs** |    **2632 B** |
     InsertIntoTableAtMiddle |        1000 | 2.467 μs | 0.0516 μs | 0.0917 μs | 2.450 μs |    2728 B |
        InsertIntoTableAtEnd |        1000 | 2.556 μs | 0.0549 μs | 0.1337 μs | 2.500 μs |    2632 B |
      DeleteFromStartOfTable |        1000 | 2.149 μs | 0.0726 μs | 0.1975 μs | 2.100 μs |     648 B |
     DeleteFromMiddleOfTable |        1000 | 2.088 μs | 0.0925 μs | 0.2562 μs | 2.000 μs |     688 B |
        DeleteFromEndOfTable |        1000 | 2.076 μs | 0.0706 μs | 0.1922 μs | 2.000 μs |     688 B |
  GetSubstringAtStartOfTable |        1000 | 2.102 μs | 0.0960 μs | 0.2723 μs | 2.000 μs |     528 B |
 GetSubstringAtMiddleOfTable |        1000 | 2.169 μs | 0.0975 μs | 0.2620 μs | 2.100 μs |     600 B |
    GetSubstringAtEndOfTable |        1000 | 2.381 μs | 0.1087 μs | 0.2938 μs | 2.300 μs |     592 B |
      **InsertIntoTableAtStart** |       **10000** | **3.116 μs** | **0.1847 μs** | **0.5087 μs** | **3.100 μs** |    **2744 B** |
     InsertIntoTableAtMiddle |       10000 | 3.651 μs | 0.1704 μs | 0.4693 μs | 3.600 μs |    2840 B |
        InsertIntoTableAtEnd |       10000 | 3.229 μs | 0.2222 μs | 0.6231 μs | 3.200 μs |    2744 B |
      DeleteFromStartOfTable |       10000 | 4.547 μs | 0.4774 μs | 1.4002 μs | 4.500 μs |     648 B |
     DeleteFromMiddleOfTable |       10000 | 4.365 μs | 0.3973 μs | 1.1526 μs | 4.200 μs |     688 B |
        DeleteFromEndOfTable |       10000 | 4.876 μs | 0.3782 μs | 1.0666 μs | 4.900 μs |     688 B |
  GetSubstringAtStartOfTable |       10000 | 3.417 μs | 0.2380 μs | 0.6753 μs | 3.300 μs |     528 B |
 GetSubstringAtMiddleOfTable |       10000 | 4.601 μs | 0.3628 μs | 1.0409 μs | 4.800 μs |     600 B |
    GetSubstringAtEndOfTable |       10000 | 4.623 μs | 0.4608 μs | 1.2922 μs | 4.500 μs |     592 B |
