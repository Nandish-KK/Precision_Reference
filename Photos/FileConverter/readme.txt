We provide two tools to convert bin file into csv file:Bin2csv.exe and Convert_bin_to_csv_file.py . 

The exe application can be used directly.
Steps:
Double click to run the exe;
Click "Browse" to select the bin file that needs to be converted;
Select the model of the bin file;
Click "Convert" to start the conversion;
(When the number of data points is large, the time of the conversion may be longer. Please be patient.)
The path of the file generated after the conversion is the path of the bin file,and named as "csv_data.csv".

The python file is to facilitate you to understand the conversion process, only for reference. 
You need to install the corresponding library files before using, and if necessary, the code needs to be modified.

Note:
1.The conversion of digital channels is not supported at present;
2.We have tested the Bin2csv.exe on the systems: WinXP(32 bit)\Win7(32\64 bit)\Win10(64 bit).
3.Support different binary format file conversion. The first byte of the file is the version number, Please use a binary file editor to confirm the binary format. 


Change log:
Bin2csv.exe(V2.0)
1.Support binary format V1.0, V2.0

Bin2csv.exe(V3.0)
1.Support for Digital
2.Separate the analog and digital channel data to save into 2 files：Analog_Trace.csv, Digital_Trace.csv

Bin2csv.exe(V3.1)
1.Cancel interface selection option: Model

Bin2csv.exe(V3.2)
1.Modify build csv file naming policy：the file name of the bin file, added with the analog/digital channel flag.
2.Such as:1k_c2_d0-7.bin ->1k_c2_d0-7_Analog_Trace.csv & 1k_c2_d0-7_Digital_Trace.csv

FileConverter.exe(V3.4)
1.Modify the application name to "FileConverter"
2.Support for Math(except FFT).

FileConverter.exe(V3.5)
1.Support to convert binary file(*.slg,*.mlg) of Data Logger.
2.Static compilation and packaging to avoid the unavailability of the application in some scenarios.
3.Support binary format V1.0, V2.0, V3.0

FileConverter.exe(V3.5.1)
1.Synchronizate the modification of the binary file header, to be compatible with the new firmware version:
2.Support binary format V1.0, V2.0, V3.0, V4.0

FileConverter.exe(V3.5.2)
1.Correct the time axis information of waveform data.In previous versions, the leftmost side of the screen was the starting point.

FileConverter.exe(V3.5.3)
1.Fixed the time axis information in fixed memory depth mode.

FileConverter.exe(V3.5.4)
1.Fix bug: horizontal time axis conversion error when the horizontal reference center is not at 50%.

FileConverter.exe(V3.5.4.1)
1.The input parameter is changed from file name to file path to support batch processing of files.

FileConverter.exe(V3.5.5)
1.Support binary format V1.0, V2.0, V3.0, V4.0, V5.0

FileConverter.exe(V3.5.6)
1.Support bin file parsing for C5~C8.
2.Support binary format V1.0, V2.0, V3.0, V4.0, V5.0, V6.0

FileConverter.exe(V3.5.7)
1.Fixed some bugs.
2.Support for Memory waveform file conversion.

FileConverter.exe(V3.5.8)
1.Resolve the first few exceptions in Zoom source conversion.