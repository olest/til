What is CPU scaling? See [here](https://wiki.archlinux.org/title/CPU_frequency_scaling).

How to check if it is enabled?
```
cat /sys/devices/system/cpu/cpu[0-9]*/cpufreq/scaling_governor
```
On my laptop, this will say powersave by default.


How to disable CPU scaling?
```
echo performance | sudo tee /sys/devices/system/cpu/cpu[0-9]*/cpufreq/scaling_governor
```

Reset to default: 
```
echo powersave | sudo tee /sys/devices/system/cpu/cpu[0-9]*/cpufreq/scaling_governor
```

