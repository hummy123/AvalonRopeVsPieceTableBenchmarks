|                 Method | stringLength |         Mean |     Error |    StdDev |    Gen0 | Allocated |
|----------------------- |------------- |-------------:|----------:|----------:|--------:|----------:|
| **CreatePieceTableOfSize** |          **100** |     **84.25 ns** |  **0.973 ns** |  **0.910 ns** |  **0.1988** |     **416 B** |
|       CreateRopeOfSize |          100 |    529.75 ns |  4.652 ns |  4.351 ns |  0.8678 |    1816 B |
| **CreatePieceTableOfSize** |         **1000** |    **277.93 ns** |  **1.495 ns** |  **1.325 ns** |  **1.0591** |    **2216 B** |
|       CreateRopeOfSize |         1000 |  2,003.23 ns |  5.272 ns |  4.402 ns |  2.7466 |    5752 B |
| **CreatePieceTableOfSize** |        **10000** |  **5,551.73 ns** | **20.291 ns** | **18.980 ns** | **29.2664** |   **61456 B** |
|       CreateRopeOfSize |        10000 | 17,488.38 ns | 64.245 ns | 60.095 ns | 23.5291 |   49384 B |
