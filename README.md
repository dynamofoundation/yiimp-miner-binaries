# yiimp-miner-binaries
binary builds of yiimp compatible miner

These binaries are compatible with yiimp pools.  The command line arguments are:

mining pool IP or name
port
your wallet address
parameters as needed by pool
GPU
number of compute units - should be a multiple of 64 and better to be a power of 2
openCL platform (varies by system, but usually 0 or 1)
number of workitems - should be one of: 32, 64, 128, 256, 512  (try them all for optimal results)

Example:
yiimp_miner eu.letshash.it 5966 dy1222222222233333333334444444444555555555.myminer d=2 GPU 32768 1 128

Hashrate performance by card will vary - you should try different combinations of compute units and work items.  Compute units should be a multiple of work items for optimal performance.
