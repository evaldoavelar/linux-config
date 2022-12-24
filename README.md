# Permanently Set NVIDIA PowerMizer Settings

we can use the -a option to set the value of GpuPowerMizerMode to 1 and verify it has been changed using the -q option:


```
$ nvidia-settings -a "[gpu:0]/GpuPowerMizerMode=1"

  Attribute 'GPUPowerMizerMode' (rastating-PC:1[gpu:0]) assigned value 1.

$ nvidia-settings -q GpuPowerMizerMode

  Attribute 'GPUPowerMizerMode' (rastating-PC:1[gpu:0]): 1.
    Valid values for 'GPUPowerMizerMode' are: 0, 1 and 2.
    'GPUPowerMizerMode' can use the following target types: GPU.
```
