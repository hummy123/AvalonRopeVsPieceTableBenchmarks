|                 Method | stringLength |         Mean |     Error |    StdDev |    Gen0 | Allocated |
|----------------------- |------------- |-------------:|----------:|----------:|--------:|----------:|
| **CreatePieceTableOfSize** |          **100** |     **84.49 ns** |  **0.792 ns** |  **0.741 ns** |  **0.1988** |     **416 B** |
|       CreateRopeOfSize |          100 |    526.69 ns |  3.347 ns |  3.131 ns |  0.8678 |    1816 B |
| **CreatePieceTableOfSize** |         **1000** |    **278.37 ns** |  **0.935 ns** |  **0.875 ns** |  **1.0591** |    **2216 B** |
|       CreateRopeOfSize |         1000 |  1,999.96 ns |  3.377 ns |  2.820 ns |  2.7466 |    5752 B |
| **CreatePieceTableOfSize** |        **10000** |  **5,538.43 ns** | **19.842 ns** | **18.560 ns** | **29.2664** |   **61456 B** |
|       CreateRopeOfSize |        10000 | 17,445.72 ns | 72.104 ns | 63.918 ns | 23.5291 |   49384 B |
