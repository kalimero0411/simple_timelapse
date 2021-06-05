# simple_timelapse
A simple bash script for creating timelapses.

```
simple_timelapse [OPTIONS]
	-d | --device	Recording device (default /dev/video0)
	-i | --interval	Interval between pictures in seconds (default 1)
	-p | --pictures	Total number of pictures to take (default 5)
	-t | --time	Total time in seconds (default 5)
	-o | --outdir	Output directory (default home directory)
	-r | --resolution	Resolution for the output pictures (default 1280x720)
	-n | --name	Base name of the pictures (default 'timelapse_pics')
	-f | --frames	Number of frames per picture (default 5)
	-v | --verbose	Verbose output (default off)
```
  
- The `--time` option overrides `--pictures`.
- If `--time` is exactly divisible by `--interval`, the picture at `--time` is NOT TAKEN.
