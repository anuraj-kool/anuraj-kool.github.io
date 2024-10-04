- miniforge
	- https://github.com/conda-forge/miniforge?tab=readme-ov-file
	- ```
	  curl -L -O "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-$(uname)-$(uname -m).sh"
	  bash Miniforge3-$(uname)-$(uname -m).sh
	  ```
	- ```
	  To activate this environment, use:
	  
	      micromamba activate /Users/wannabe/miniforge3
	  
	  Or to execute a single command in this environment, use:
	  
	      micromamba run -p /Users/wannabe/miniforge3 mycommand
	  
	  
	  ```
- ```
  conda config --set auto_activate_base False
  ```
- ```
  anuraj.kool$ conda create -n pyml python=3.9
  anuraj.kool$ conda activate pyml
  (pyml) anuraj.kool$ conda install numpy scipy scikit-learn matplotlib pandas jupyter
  ```
-
-