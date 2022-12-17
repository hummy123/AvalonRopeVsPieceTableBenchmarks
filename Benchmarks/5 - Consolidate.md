``` ini

BenchmarkDotNet=v0.13.2, OS=Windows 11 (10.0.22000.1335/21H2)
AMD Ryzen 3 5300U with Radeon Graphics, 1 CPU, 8 logical and 4 physical cores
.NET SDK=7.0.101
  [Host]     : .NET 6.0.11 (6.0.1122.52304), X64 RyuJIT AVX2 DEBUG
  Job-SEDMFQ : .NET 6.0.11 (6.0.1122.52304), X64 RyuJIT AVX2

InvocationCount=1  UnrollFactor=1  

```
|           Method |  size |       Mean |      Error |     StdDev |     Median |
|----------------- |------ |-----------:|-----------:|-----------:|-----------:|
| **ConsolidateTable** |   **100** |   **2.188 μs** |  **0.0472 μs** |  **0.0485 μs** |   **2.200 μs** |
| **ConsolidateTable** |  **1000** |  **24.393 μs** |  **1.5097 μs** |  **4.4038 μs** |  **23.650 μs** |
| **ConsolidateTable** | **10000** | **442.085 μs** | **18.5936 μs** | **53.0485 μs** | **420.450 μs** |
