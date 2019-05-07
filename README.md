# SIngularity Container

This is a beginner tutorial on using SIngularity COntainers

# Setup

Navigate to rc.uab.edu in your preferred web browser and login. 

From the dashboard, click "Jobs" and then "Job Composer" to open the job composer.

Create a new job from the default template. Then scroll down the page and select "Open Editor" at the bottom under "Submit Script"

Copy and paste the following code into the editor window. (Replace all current code with the pasted code)
```
#!/bin/bash
# JOB HEADERS HERE
mkdir -p /data/user/$USER/rc-training-sessions
git clone https://gitlab.rc.uab.edu/rc-training-sessions/singularity_containers.git /data/user/$USER/rc-training-sessions/singularity_containers


```

# Start Jupyter Notebook 
Launch Jupyter Notebook through the interactive apps page in the OnDemand (rc.uab.edu) portal using following settings:

## Environment Setup:
```
# Load required modules
module load Singularity/2.5.2-GCC-5.4.0-2.26
module load Anaconda3
```

## Extra Jupyter Arguments:
```
--notebook-dir=/data/user/$USER/rc-training-sessions/singularity_containers
```
