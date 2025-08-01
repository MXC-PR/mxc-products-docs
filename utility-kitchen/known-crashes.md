# Known Crashes

## ScaleformStore Pool Full, Size == 852

When the Scaleform pool becomes full, it can lead to crashes because the system is unable to allocate additional resources beyond its capacity. \
To increase the pool size add the following line to your `server.cfg` configuration file:

```lua
increase_pool_size "ScaleformStore" 200
```

