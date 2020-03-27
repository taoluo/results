# results
[global]

ioengine=io_uring
fixedbufs=1
registerfiles=1
hipri=1  

thread=1 

iodepth=1024
bs=4096
direct=1

group_reporting=1

size=1Gi

#lat_percentiles=1
#percentile_list=50:99:99.9

time_based=1
ramp_time=3
clocksource=cpu

rw=randread
stonewall

[run]
runtime=10
filename=/dev/nvme0n1
rate_iops=500000
rate_iops_min=100000

numjobs=1

ioengine=io_uring
hipri=1
sqthread_poll=1









