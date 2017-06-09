# HDF5Mathematica
HDF5 interface for Mathematica

INSTRUCTIONS:

- Everything should be all set up and ready to go (*). 

- Just open "1 crtfile.nb" in the folder of Basic Tutorial to start doing some examples.

- In case of any .NET errors, see 'TROUBLESHOOTING' for two common issues.

- Folders & Files:

--- Folder "HDF5 Basic Tutorial (start here)": Files listed as "1...", "2...", in that folder correspond to tutorial examples: http://www.hdfgroup.org/HDF5/Tutor/introductory.html. In each, the accompanying 'C' code is included for direct comparison between implementation in 'C' and that in Mathematica.

--- Folders "HDF5 Intermediate Tutorial", "HDF5 Advanced Tutorial",  and "HDF5 Real Case Studies" provide progressively more advanced demonstrations of using Mathematica with HDF5 files.

--- Folder "HDF5.Mathematica.Packages" contains the Mathematica packages for HDF5 implementation. "HDF5.nb" is the main package for Mathematica wrappers that correspond on a one-to-one basis with the functions of the HDF5group (http://www.hdfgroup.org/HDF5/doc/RM/). "HDF5Basic.nb" upgrades the basic one-to-one functions by taking care of some aspects of the technical interface, such as System.IntPtr on some functions. "HDF5Extend.nb" extends some of the basic functions so that they are called and provide returns in a format more similar to normal Mathematica syntax. In principle, this package adds convenience but no new functionality. "HDF5HighLevel.nb" extends further "HDF5Extend.nb" with some higher level functions that acts as small programs and work on complete HDF5 files. 

--- These demonstrations were last prepared and run on Windows 10, 64 bit, using Mathematica 11.0.0.

(*) Note that provided files are for Windows10, 64 bit. This related to the DLL library of "C". For use on a 32 bit machine, swap the DLL files in the PInvoke directory (it should be straightforward based on folder names).

First version of these packages was released by Scot Martin, 14 July 2011, scot_martin@harvard.edu. Current version was released 12 August 2016.

Acknowledgments: This material is based upon work supported by the National Science Foundation. Any opinions, finndings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.

UPDATES:
8 June 2017, version 2.01. Major: The option "ByteRead" was added for H5DExtendRead functions. Minor: Additional H5 library functions implemented, including H5TgetEBias, H5TgetFields, H5TgetInPad, H5TgetNorm, H5TgetOffset, H5TgetOrder, H5TgetPad, H5TgetPrecision, and H5TgetSign, along with some corresponding H5TBasicGet... functions.
