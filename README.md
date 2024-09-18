### Trajectory and Log Data Processing for Molecular Dynamics Simulations

##### Overview

This repository provides a Python module for reading, processing, and extracting data from ReaxFF molecular dynamics simulations. The code is designed to work with output files generated from MD simulations, including trajectory files (atom positions, velocities, etc.) and log files (thermodynamic properties such as temperature, potential energy, and pressure). The primary functionalities of this module include:

	•	Reading trajectory files with atomic information over different timesteps.
	•	Reading log files that record global properties over simulation time.
	•	Extracting specific data from both types of files using projections for post-analysis.

Features

	1.	Trajectory Data Processing:
	•	The read_reax_traj function reads trajectory data from a ReaxFF MD simulation, parsing information about atomic positions, velocities, and atom types over multiple timesteps.
	2.	Log Data Processing:
	•	The read_reax_log_traj function reads log data from ReaxFF simulations, which records thermodynamic properties such as temperature, potential energy, and pressure over time.
	3.	Data Projections:
	•	The projections function allows for the extraction of specific values (e.g., coordinates, atom types, thermodynamic properties) at selected timesteps and for specified atoms.
	•	Users can control the depth of the extraction to customize how nested the output should be (single values, lists, or deep flattened structures).

