# TG-43--Dose-Rate-calculator

The TG-43 Dose Rate Calculator is a web-based tool designed to compute dose rates for brachytherapy sources using the TG-43 formalism. This tool allows users to calculate dose distributions for both point source and line source approximations, based on user-provided input parameters such as calculation coordinates, dwell position, dwell time, and activity.

The calculator reads radial dose function and anisotropy function data from an uploaded Excel file, interpolates values, and applies TG-43 equations to compute:
	•	Distance (r) between source and calculation point
	•	Angle (θ) relative to the source
	•	Radial Dose Function (g_L(r))
	•	Anisotropy Function (F(r,θ))
	•	Geometrical Factor (G_L(r,θ))
	•	Dose Rate (D(r,θ)) in cGy/hr
	•	Total Dose received at the calculation point

Features

 Supports both point source and line source calculations
 Reads and interpolates dose data from an Excel file
 Calculates geometrical factors, radial dose, and anisotropy functions
 Provides total dose estimation based on dwell time and source activity
 Uses JavaScript and the XLSX library to handle Excel file parsing

How to Use
	1.	Select the source type (Point or Line).
	2.	Enter the calculation coordinates (x, y, z) and dwell position (x, y, z).
	3.	Input dwell time (seconds) and source activity (mCi).
	4.	Upload an Excel file containing interpolated anisotropy and radial dose function data.
	5.	Click “Calculate” to compute results.
	6.	View computed values for distance, angle, dose rate, and total dose in the results section.

Requirements
	•	Web browser (Chrome, Firefox, Edge, etc.)
	•	Excel file containing precomputed dose function data
	•	Internet connection (for loading the XLSX library)

