|                  Method | insertTimes |       Mean |     Error |     StdDev |     Median | Allocated |
|------------------------ |------------ |-----------:|----------:|-----------:|-----------:|----------:|
|  **DeleteFromStartOfTable** |         **100** |   **1.982 μs** | **0.0326 μs** |  **0.0563 μs** |   **2.000 μs** |     **792 B** |
|   DeleteFromStartOfRope |         100 |   5.167 μs | 0.0631 μs |  0.0492 μs |   5.200 μs |     880 B |
| DeleteFromMiddleOfTable |         100 |   6.518 μs | 0.1124 μs |  0.1611 μs |   6.500 μs |    9320 B |
|  DeleteFromMiddleOfRope |         100 |   5.120 μs | 0.0921 μs |  0.0862 μs |   5.100 μs |     880 B |
|    DeleteFromEndOfTable |         100 |  10.267 μs | 0.2047 μs |  0.1915 μs |  10.300 μs |   17384 B |
|     DeleteFromEndOfRope |         100 |   5.227 μs | 0.1023 μs |  0.1947 μs |   5.200 μs |     872 B |
|  **DeleteFromStartOfTable** |        **1000** |   **3.257 μs** | **0.4089 μs** |  **1.1666 μs** |   **2.700 μs** |     **792 B** |
|   DeleteFromStartOfRope |        1000 |   6.794 μs | 0.3923 μs |  1.0605 μs |   6.400 μs |    1000 B |
| DeleteFromMiddleOfTable |        1000 |  42.072 μs | 0.8388 μs |  1.1197 μs |  42.300 μs |   84920 B |
|  DeleteFromMiddleOfRope |        1000 |   7.046 μs | 0.3609 μs |  0.9633 μs |   6.800 μs |    1000 B |
|    DeleteFromEndOfTable |        1000 |  78.174 μs | 1.5594 μs |  1.7333 μs |  78.200 μs |  168584 B |
|     DeleteFromEndOfRope |        1000 |   6.454 μs | 0.1300 μs |  0.3424 μs |   6.400 μs |     992 B |
|  **DeleteFromStartOfTable** |       **10000** |   **5.285 μs** | **0.5031 μs** |  **1.4353 μs** |   **4.550 μs** |     **792 B** |
|   DeleteFromStartOfRope |       10000 |  12.602 μs | 0.3518 μs |  0.9863 μs |  12.300 μs |    1160 B |
| DeleteFromMiddleOfTable |       10000 | 238.190 μs | 3.9170 μs |  4.5108 μs | 238.000 μs |  840920 B |
|  DeleteFromMiddleOfRope |       10000 |  13.359 μs | 0.4687 μs |  1.3066 μs |  12.950 μs |    1160 B |
|    DeleteFromEndOfTable |       10000 | 493.740 μs | 9.7198 μs | 11.1934 μs | 492.900 μs | 1680584 B |
|     DeleteFromEndOfRope |       10000 |  12.220 μs | 0.3643 μs |  1.0335 μs |  11.750 μs |    1152 B |
