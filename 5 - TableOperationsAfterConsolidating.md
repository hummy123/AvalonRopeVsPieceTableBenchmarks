|                      Method | insertTimes |     Mean |     Error |    StdDev |   Median | Allocated |
|---------------------------- |------------ |---------:|----------:|----------:|---------:|----------:|
|      **InsertIntoTableAtStart** |         **100** | **2.127 μs** | **0.0455 μs** | **0.0908 μs** | **2.100 μs** |    **1712 B** |
|     InsertIntoTableAtMiddle |         100 | 2.594 μs | 0.0845 μs | 0.2326 μs | 2.550 μs |    1808 B |
|        InsertIntoTableAtEnd |         100 | 2.171 μs | 0.0356 μs | 0.0642 μs | 2.200 μs |    1712 B |
|      DeleteFromStartOfTable |         100 | 1.796 μs | 0.0396 μs | 0.1037 μs | 1.800 μs |     648 B |
|     DeleteFromMiddleOfTable |         100 | 2.253 μs | 0.0892 μs | 0.2473 μs | 2.200 μs |     688 B |
|        DeleteFromEndOfTable |         100 | 1.927 μs | 0.0420 μs | 0.0788 μs | 1.900 μs |     688 B |
|  GetSubstringAtStartOfTable |         100 | 1.819 μs | 0.0613 μs | 0.1758 μs | 1.800 μs |     528 B |
| GetSubstringAtMiddleOfTable |         100 | 2.005 μs | 0.0457 μs | 0.1297 μs | 2.000 μs |     600 B |
|    GetSubstringAtEndOfTable |         100 | 2.026 μs | 0.0515 μs | 0.1444 μs | 2.000 μs |     592 B |
|      **InsertIntoTableAtStart** |        **1000** | **2.524 μs** | **0.0539 μs** | **0.1026 μs** | **2.500 μs** |    **2632 B** |
|     InsertIntoTableAtMiddle |        1000 | 2.663 μs | 0.0587 μs | 0.1656 μs | 2.600 μs |    2728 B |
|        InsertIntoTableAtEnd |        1000 | 2.436 μs | 0.0518 μs | 0.0822 μs | 2.400 μs |    2632 B |
|      DeleteFromStartOfTable |        1000 | 2.223 μs | 0.0689 μs | 0.1933 μs | 2.200 μs |     648 B |
|     DeleteFromMiddleOfTable |        1000 | 2.526 μs | 0.1969 μs | 0.5681 μs | 2.300 μs |     688 B |
|        DeleteFromEndOfTable |        1000 | 2.240 μs | 0.0611 μs | 0.1723 μs | 2.200 μs |     688 B |
|  GetSubstringAtStartOfTable |        1000 | 1.818 μs | 0.0400 μs | 0.0869 μs | 1.800 μs |     528 B |
| GetSubstringAtMiddleOfTable |        1000 | 2.243 μs | 0.0483 μs | 0.1339 μs | 2.200 μs |     600 B |
|    GetSubstringAtEndOfTable |        1000 | 2.367 μs | 0.0941 μs | 0.2622 μs | 2.300 μs |     592 B |
|      **InsertIntoTableAtStart** |       **10000** | **2.986 μs** | **0.2126 μs** | **0.6135 μs** | **2.800 μs** |    **2744 B** |
|     InsertIntoTableAtMiddle |       10000 | 3.734 μs | 0.1431 μs | 0.4012 μs | 3.700 μs |    2840 B |
|        InsertIntoTableAtEnd |       10000 | 3.180 μs | 0.1953 μs | 0.5540 μs | 3.100 μs |    2744 B |
|      DeleteFromStartOfTable |       10000 | 4.357 μs | 0.4364 μs | 1.2729 μs | 4.600 μs |     648 B |
|     DeleteFromMiddleOfTable |       10000 | 4.422 μs | 0.4241 μs | 1.2372 μs | 4.300 μs |     688 B |
|        DeleteFromEndOfTable |       10000 | 4.546 μs | 0.3903 μs | 1.1323 μs | 4.700 μs |     688 B |
|  GetSubstringAtStartOfTable |       10000 | 3.219 μs | 0.2088 μs | 0.6025 μs | 3.050 μs |     528 B |
| GetSubstringAtMiddleOfTable |       10000 | 4.594 μs | 0.3497 μs | 1.0200 μs | 4.600 μs |     600 B |
|    GetSubstringAtEndOfTable |       10000 | 4.486 μs | 0.4135 μs | 1.2063 μs | 4.500 μs |     592 B |
