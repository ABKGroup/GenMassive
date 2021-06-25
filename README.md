# GenMassive
The GenMassive repository contains the generation scripts for large-scale "Designs of Experiments" (DOEs) runs, which generates config files and runscripts of experiments to use for the open-source RTL-to-GDS flow of the [OpenROAD tool](https://github.com/The-OpenROAD-Project).

The genMassive.py script can be placed under flow/util/ in the [OpenROAD-flow-scripts](https://github.com/The-OpenROAD-Project/OpenROAD-flow-scripts).

For brief instructions on how to use, refer to the following ppt slides [here](https://drive.google.com/file/d/1xbp4KJl3Hzyj9CMTodseSRms1rxTeZyN/view?usp=sharing).

## ChangeLogs
### commit 98108defe2b5b7faeb38bccfe9ccd2b5008d7f82
  - Now it uses {chunks/chunk0, chunks/chunk1, ...,} directory under the design directory to reduce the burden on the file reading. The number of runs per chunk can be set as the NumFilesPerChunk variable in genMassive.py.
  - The lower boundary for PLACE_DENSITY is now calculated in the OR tool.
  - Sweeping GR seed is enabled.
  - Sweeping DR seed is enabled.
  - Sweeping clock uncertainty, IO delay are enabled.
  - Original sdc name can be defined as a template.


