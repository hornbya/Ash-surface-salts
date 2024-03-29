# Surface salts analysis macro
Segmentation and analysis of salts on glass particles

Further details in the publication:
Casas, A.S., Hornby, A., Poetsch, C. et al. A novel method for the quantitative morphometric characterization of soluble salts on volcanic ash. Bull Volcanol 84, 3 (2022). https://doi.org/10.1007/s00445-021-01519-3

***********************************************************************
AGAR salts analysis for high-magnification SEM images

The macro segments background, salts and adhering particles, then measures the size, shape and coverage (area %) of the salts.
Output files are saved in separate folders for each image, using the image file name as title.
MorphoLibJ https://imagej.net/MorphoLibJ (doi.org/10.1093/bioinformatics/btw413) Shape Filter https://imagej.net/Shape_Filter (http://dx.doi.org/10.5334/jors.ae) and Read and Write Excel (https://imagej.net/User:ResultsToExcel) plugins are required.

MorphoLibJ is used for greyscale smoothing, opening and closing operations.

Shape Filter is used to measure the salts' dimensions, giving improved perimeter estimation to Analyze Particles.
Default settings: No filtered values. Size filtering at minimum 5 pixels is done prior to measurement.

Read and Write Excel is used to arrange and collate results columns from the shape data output into labelled tabs in an Excel sheet. 
Default settings: Shape results data within subfolders of the selected input directory are processed in sequence. 
Shape columns extracted are: Area, Perimeter, Solidity, Form factor, Roundness, Feret diameter and Orientation.
Final arranged Excel file is saved on the desktop as 'Rename me after writing is done.xlsx".

A menu tool can be installed: (1) Move all macros to the default macros folder (e.g. ...fiji-win64\Fiji.app\macros). (2) Move 'Salts AGAR menu tool.txt' to the toolset folder (...fiji-win64\Fiji.app\macros\toolsets). (3) Open ImageJ and the menu tool can be found by clicking on the >> button.


This project has received funding from the European Union's Horizon 2020 research and innovation programme
