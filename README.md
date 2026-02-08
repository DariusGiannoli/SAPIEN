# Sapien Project 

Team members: 
- Darius Giannoli (Teleoperation)
- Joelle Ayoub (Mechanics)
- Edoaordo Tadini (Electronics)
- Alexandre Huou (Reinforcement Learning)
- Karol Wickel (Electronics)
- Tristan Carron (Mechanics)

## Berkeley Humanoid Lite

[![Python](https://img.shields.io/badge/python-3.10-blue.svg)](https://docs.python.org/3/whatsnew/3.10.html)
[![License](https://img.shields.io/badge/license-MIT-yellow.svg)](https://opensource.org/license/mit)
[![License](https://img.shields.io/badge/license-CC%20BY--SA%204.0-orange.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

**[Website](http://lite.berkeley-humanoid.org/)** | **[arXiv](https://arxiv.org/abs/2504.17249)** | **[Paper](https://lite.berkeley-humanoid.org/static/paper/demonstrating-berkeley-humanoid-lite.pdf)** | **[Video](https://youtu.be/dIdJGkMDFl4?si=SRD7HhQQbhM3JCRA)** | **[Documentation](https://berkeley-humanoid-lite.gitbook.io/berkeley-humanoid-lite-docs)** | **[Releases](https://berkeley-humanoid-lite.gitbook.io/docs/releases)**


## Overview

This repository is the workspace for the Berkeley Humanoid Lite project that contains everything we need, including policy training, sim2sim validation, real-world deployment, motion capture, and teleoperated manipulation controls.

Functionalities are organized into several submodules. We arrange the directory structure following the Isaac Lab convention, where each submodule can be installed as an extension:

- `source/berkeley_humanoid_lite/` contains the IsaacLab environment and task definitions.

- `source/berkeley_humanoid_lite_assets/` contains robot descriptions (URDF, MJCF, and USD) and the script to export these description files from Onshape project.

- `source/berkeley_humanoid_lite_lowlevel/` contains the lowlevel code running on the real robot. Only contents inside this folder is required to deploy to the real robot.

Except a few edge cases, all the commands should be invoked from the root directory of this repository. The entry points of different flows are collected in the `scripts/` directory.



