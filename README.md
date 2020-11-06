# dicomtojpegconverter

this little PYTHON code works on Jupyter notebook.
converts crazy named dicom files like "1.2.840.113619.2.80.3826548172.22009.1603090100.6" to anonymized jpeg files. 

Number 6 at the end of example file is file extension (not .dcm or dicom). Actually this file is a dicom file with metadata and pixel compressed JPEG 2000 Lossless Synthax.

WHAT THIS CODE DOES?

1. scans all files in the directory in which, this code also has to be in. and return a list.
2. picks the file names contain multiple dots ("." string) from the list.
3. reads the dicom files
4. picks pixel info
5. converts it into numpyArray
6. downsamples it x8 times
7. and saves as jpeg file with same name.

I hope this code will be practical for AI practitioners when preparing training data set for their models.


CREDITS GO TO
            ***** PYDICOM
            ***** NUMPY
            ***** MATPLOTLIB
