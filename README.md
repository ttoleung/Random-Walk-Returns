# Random-Walk-Returns
Marks a random investment return but tracks toward a benchmark.
This is useful when you provide a dummy investment product to your clients, and wants to look different from other investment products.

Given Variables
- t: tolernece (e.g. 0.025, diverge up to 2.5% from benchmark)
- bm: benchmark return (e.g. SPY returns)
- cr: current cumulated return

Then
Trailing return, tr = cr - br
Proposed return, p = random( min(-t, tr-t), max(t, tr+t) )
