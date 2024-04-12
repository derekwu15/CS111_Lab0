# A Kernel Seedling
TODO: intro
A kernel module that creates a /proc/count file that reports the number of running processes. When the module loads and unloads, it will in turn create or remove the /proc/count file. The following will detail how to build, run, test, and clean up the module. 

## Building
```shell
TODO: cmd for build
make
```

## Running
```shell
TODO: cmd for running binary

sudo insmod proc_count.ko
cat /proc/count
```
TODO: results?
Running cat /proc/count will provide an integer result for the number of processes

## Cleaning Up
```shell
TODO: cmd for cleaning the built binary
sudo rmmod proc_count.ko
```

## Testing
```python
python -m unittest
```
TODO: results?
Sample test result provided below: 

Ran 3 tests in 18.715s

OK 

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
TODO: kernel ver?
Linux 5.14.8-arch1-1 #1 SMP PREEMPT