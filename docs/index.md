<figure markdown>
![IWH5 Title](../assets/images/Graphics/iwh5-title.png){ width="800" }
</figure>

# Overview

Welcome to the official documentation for the `.iwh5`, which utilizes an HDF5 container combined with JSON metadata to store nondestructive evaluation (NDE) data. This guide provides a complete overview of our file structures, specifications, usage guidelines, and integration instructions. Whether you're a developer, partner, or internal team member, this resource will help you understand how to create, read, and validate files in our formats efficiently.

# What is HDF5?

A high performance data file format for:

- **Easy sharing**: Portable and no vendor lock-in
- **Cross platform**: APIs available in C++, C#, Python, Java, etc.
- **Fast**: Quick access and optimized storage
- **Large Data**: No restriction on file size and built-in compression
- **Embedded Metadata**: Describes how the data was collected and analyzed

Who maintains HDF5?

Supported by **The HDF Group®**, a non-profit organization that ensures:

- **Continued Technological** development
- **Continued Accessibility** of data stored in HDF

# What is iwh5?

An InspectionWare data file format that stores:

- NDT Data, in the hdf5 format  
- Inspection Metadata, in the Json format  
- Analysis Results, in the Json format  
- Structural Information, for compatibility with InspectionWare applications
