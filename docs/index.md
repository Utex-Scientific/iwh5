![IWH5 Title](assets/images/Graphics/iwh5-title.png)

# Overview

This site provdies the official documentation for reading and writing `.iwh5` file format, which utilizes an HDF5 container combined with JSON metadata to store nondestructive evaluation (NDE) data. The guide provides an overview of the file structures, specifications, usage guidelines, and integration instructions. Whether you're a developer, academic or industrial partner, or internal team member, this resource will help you understand how to create, read, and validate files in our formats efficiently.

# What is HDF5?

A high performance data file format for:

- **Easy sharing**: Portable and no vendor lock-in
- **Cross platform**: APIs available in multiple programming languages.
- **Fast**: Quick access and optimized storage
- **Large Data**: No restriction on file size with built-in compression
- **Embedded Metadata**: Describes how the data was collected and analyzed

!!! question "Who maintains HDF5?"
    Supported by [**The HDF Group®**](https://www.hdfgroup.org/), a non-profit organization that ensures:

    - **Continued Technological** development
    - **Continued Accessibility** of data stored in HDF

# What is iwh5?

An InspectionWare data file format that stores:

- NDT Data, in the hdf5 format  
- Inspection Metadata, in the Json format  
- Analysis Results, in the Json format  
- Structural Information, for compatibility with InspectionWare applications
