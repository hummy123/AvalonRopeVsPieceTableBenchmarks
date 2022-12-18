|                      Method | insertTimes |       Mean |     Error |    StdDev |     Median | Allocated |
|---------------------------- |------------ |-----------:|----------:|----------:|-----------:|----------:|
|  **GetSubstringAtStartOfTable** |         **100** |   **2.168 μs** | **0.0430 μs** | **0.0478 μs** |   **2.200 μs** |     **736 B** |
|   GetSubstringAtStartOfRope |         100 |   1.890 μs | 0.0356 μs | 0.0632 μs |   1.900 μs |     576 B |
| GetSubstringAtMiddleOfTable |         100 |   5.204 μs | 0.1048 μs | 0.1503 μs |   5.100 μs |    5904 B |
|  GetSubstringAtMiddleOfRope |         100 |   1.776 μs | 0.0327 μs | 0.0436 μs |   1.800 μs |     576 B |
|    GetSubstringAtEndOfTable |         100 |   7.388 μs | 0.1475 μs | 0.1918 μs |   7.300 μs |    7912 B |
|     GetSubstringAtEndOfRope |         100 |   1.831 μs | 0.0400 μs | 0.0668 μs |   1.800 μs |     568 B |
|  **GetSubstringAtStartOfTable** |        **1000** |   **3.214 μs** | **0.1310 μs** | **0.3587 μs** |   **3.100 μs** |     **736 B** |
|   GetSubstringAtStartOfRope |        1000 |   3.546 μs | 0.3753 μs | 1.0830 μs |   3.100 μs |     576 B |
| GetSubstringAtMiddleOfTable |        1000 |  37.760 μs | 0.7434 μs | 0.9925 μs |  37.600 μs |   55024 B |
|  GetSubstringAtMiddleOfRope |        1000 |   3.496 μs | 0.4522 μs | 1.3263 μs |   2.900 μs |     576 B |
|    GetSubstringAtEndOfTable |        1000 |  57.788 μs | 0.5163 μs | 0.5071 μs |  57.700 μs |   72712 B |
|     GetSubstringAtEndOfRope |        1000 |   2.944 μs | 0.1318 μs | 0.3629 μs |   2.900 μs |     568 B |
|  **GetSubstringAtStartOfTable** |       **10000** |   **6.322 μs** | **0.2503 μs** | **0.6936 μs** |   **6.100 μs** |     **736 B** |
|   GetSubstringAtStartOfRope |       10000 |   5.285 μs | 0.2090 μs | 0.5964 μs |   5.200 μs |     576 B |
| GetSubstringAtMiddleOfTable |       10000 | 217.673 μs | 4.0266 μs | 3.7665 μs | 218.900 μs | 1078080 B |
|  GetSubstringAtMiddleOfRope |       10000 |   5.387 μs | 0.2742 μs | 0.7780 μs |   5.200 μs |     576 B |
|    GetSubstringAtEndOfTable |       10000 | 237.905 μs | 2.4219 μs | 4.4891 μs | 236.500 μs |  720712 B |
|     GetSubstringAtEndOfRope |       10000 |   5.310 μs | 0.2748 μs | 0.7929 μs |   5.100 μs |     568 B |
