
BenchmarkDotNet=v0.13.2, OS=Windows 11 (10.0.22000.1335/21H2)
AMD Ryzen 3 5300U with Radeon Graphics, 1 CPU, 8 logical and 4 physical cores
.NET SDK=7.0.101
  [Host]     : .NET 6.0.11 (6.0.1122.52304), X64 RyuJIT AVX2 DEBUG
  Job-RNPGDU : .NET 6.0.11 (6.0.1122.52304), X64 RyuJIT AVX2

InvocationCount=1  UnrollFactor=1  

                      Method | insertTimes |     Mean |     Error |    StdDev |   Median | Allocated |
---------------------------- |------------ |---------:|----------:|----------:|---------:|----------:|
  **GetSubstringAtStartOfTable** |         **100** | **1.839 μs** | **0.0651 μs** | **0.1781 μs** | **1.800 μs** |     **528 B** |
   GetSubstringAtStartOfRope |         100 | 1.985 μs | 0.0850 μs | 0.2385 μs | 1.900 μs |     576 B |
 GetSubstringAtMiddleOfTable |         100 | 2.112 μs | 0.0675 μs | 0.1870 μs | 2.100 μs |     600 B |
  GetSubstringAtMiddleOfRope |         100 | 2.035 μs | 0.1370 μs | 0.3728 μs | 1.900 μs |     576 B |
    GetSubstringAtEndOfTable |         100 | 2.170 μs | 0.0543 μs | 0.1495 μs | 2.100 μs |     592 B |
     GetSubstringAtEndOfRope |         100 | 1.964 μs | 0.0466 μs | 0.1314 μs | 1.900 μs |     568 B |
  **GetSubstringAtStartOfTable** |        **1000** | **2.721 μs** | **0.1839 μs** | **0.4972 μs** | **2.600 μs** |     **528 B** |
   GetSubstringAtStartOfRope |        1000 | 2.593 μs | 0.2291 μs | 0.6310 μs | 2.400 μs |     576 B |
 GetSubstringAtMiddleOfTable |        1000 | 3.351 μs | 0.4399 μs | 1.2693 μs | 2.900 μs |     600 B |
  GetSubstringAtMiddleOfRope |        1000 | 3.300 μs | 0.3099 μs | 0.8537 μs | 3.000 μs |     576 B |
    GetSubstringAtEndOfTable |        1000 | 3.823 μs | 0.5885 μs | 1.7168 μs | 3.100 μs |     592 B |
     GetSubstringAtEndOfRope |        1000 | 3.060 μs | 0.1441 μs | 0.3921 μs | 2.950 μs |     568 B |
  **GetSubstringAtStartOfTable** |       **10000** | **5.741 μs** | **0.3648 μs** | **1.0349 μs** | **5.600 μs** |     **528 B** |
   GetSubstringAtStartOfRope |       10000 | 4.780 μs | 0.2376 μs | 0.6701 μs | 4.600 μs |     576 B |
 GetSubstringAtMiddleOfTable |       10000 | 6.251 μs | 0.5154 μs | 1.4706 μs | 5.900 μs |     600 B |
  GetSubstringAtMiddleOfRope |       10000 | 5.627 μs | 0.3337 μs | 0.9356 μs | 5.400 μs |     576 B |
    GetSubstringAtEndOfTable |       10000 | 6.288 μs | 0.5230 μs | 1.5005 μs | 5.800 μs |     592 B |
     GetSubstringAtEndOfRope |       10000 | 4.984 μs | 0.2764 μs | 0.7797 μs | 4.950 μs |     568 B |
