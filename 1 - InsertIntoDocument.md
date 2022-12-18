|                  Method | insertTimes |      Mean |     Error |    StdDev |    Median | Allocated |
|------------------------ |------------ |----------:|----------:|----------:|----------:|----------:|
|  **InsertIntoTableAtStart** |         **100** |  **2.293 μs** | **0.0301 μs** | **0.0267 μs** |  **2.300 μs** |    **1808 B** |
|   InsertIntoRopeAtStart |         100 |  4.852 μs | 0.0995 μs | 0.1918 μs |  4.800 μs |     816 B |
| InsertIntoTableAtMiddle |         100 |  2.347 μs | 0.0849 μs | 0.2310 μs |  2.300 μs |    1712 B |
|  InsertIntoRopeAtMiddle |         100 |  4.858 μs | 0.0660 μs | 0.0515 μs |  4.900 μs |    1984 B |
|    InsertIntoTableAtEnd |         100 |  2.332 μs | 0.0505 μs | 0.1240 μs |  2.300 μs |    1712 B |
|     InsertIntoRopeAtEnd |         100 |  4.867 μs | 0.0834 μs | 0.0651 μs |  4.900 μs |    1984 B |
|  **InsertIntoTableAtStart** |        **1000** |  **3.266 μs** | **0.2362 μs** | **0.6545 μs** |  **3.000 μs** |    **2728 B** |
|   InsertIntoRopeAtStart |        1000 |  6.499 μs | 0.5178 μs | 1.4519 μs |  5.900 μs |     936 B |
| InsertIntoTableAtMiddle |        1000 |  3.333 μs | 0.2407 μs | 0.6629 μs |  3.200 μs |    2632 B |
|  InsertIntoRopeAtMiddle |        1000 |  6.537 μs | 0.4888 μs | 1.3544 μs |  6.000 μs |    2104 B |
|    InsertIntoTableAtEnd |        1000 |  4.546 μs | 0.6585 μs | 1.9208 μs |  3.500 μs |    2632 B |
|     InsertIntoRopeAtEnd |        1000 |  6.038 μs | 0.4252 μs | 1.1783 μs |  5.700 μs |    2104 B |
|  **InsertIntoTableAtStart** |       **10000** |  **6.886 μs** | **0.3784 μs** | **1.0796 μs** |  **6.600 μs** |    **2840 B** |
|   InsertIntoRopeAtStart |       10000 | 12.961 μs | 0.3555 μs | 1.0258 μs | 12.900 μs |    1096 B |
| InsertIntoTableAtMiddle |       10000 |  5.956 μs | 0.2061 μs | 0.5746 μs |  5.800 μs |    2744 B |
|  InsertIntoRopeAtMiddle |       10000 | 11.965 μs | 0.3463 μs | 0.9422 μs | 11.700 μs |    2264 B |
|    InsertIntoTableAtEnd |       10000 |  6.391 μs | 0.2922 μs | 0.8384 μs |  6.150 μs |    2744 B |
|     InsertIntoRopeAtEnd |       10000 | 12.131 μs | 0.4851 μs | 1.3362 μs | 11.800 μs |    2264 B |
