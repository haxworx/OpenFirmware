# OpenFirmware Library (ofapi)

Welcome to the OpenFirmware Library (ofapi), a userspace library designed for parsing Open-Firmware Device Trees. This library mirrors the Linux kernel's internal API for device tree parsing, facilitating hardware analysis on platforms such as POWER, SPARC, and ARM devices that support device trees.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Directory Structure](#directory-structure)
- [Contributing](#contributing)
- [License](#license)

## Overview

Originally developed in the 2000s, ofapi provides a robust interface for interacting with Open-Firmware Device Trees in user space. It is available in Debian and Ubuntu distributions as `libofapi` and `libofapi-dev`. Notably, applications like Pommed and others have integrated this library to enhance hardware interaction capabilities.

## Features

- **Device Tree Parsing**: Efficiently parse and interpret device trees on supported hardware platforms.
- **Compatibility**: Supports POWER, SPARC, and ARM architectures.
- **Integration**: Utilized by various applications for hardware management and configuration.

## Installation

### From Package Manager

For Debian and Ubuntu users, install the library using `apt`:

```bash
sudo apt-get update
sudo apt-get install libofapi libofapi-dev
```

### From Source

To build and install from source:

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/haxworx/OpenFirmware.git
   cd OpenFirmware
   ```

2. **Compile the Library**:

   ```bash
   make
   ```

3. **Install the Library**:

   ```bash
   sudo make install
   ```

## Usage

After installation, you can link the library in your projects to parse and interact with Open-Firmware Device Trees. Refer to the `example` directory for sample code demonstrating the library's usage.

## Directory Structure

- `lib/`: Contains the core library source code.
- `example/`: Provides example applications demonstrating how to use the library.
- `Makefile`: Build script for compiling the library and examples.
- `LICENSE`: License information for the project.
- `README.md`: This readme file.

## Contributing

We welcome contributions to enhance the library's functionality and compatibility. To contribute:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes with clear and concise messages.
4. Submit a pull request to the main repository.

Please ensure that your contributions adhere to the project's coding standards and include appropriate documentation.

## License

This project is licensed under the GPL-2.0 License. For more details, refer to the `LICENSE` file in the repository.

---

We appreciate your interest in the OpenFirmware Library. For any questions or support, please open an issue in the GitHub repository.

---

### Additional Notes

#### Device Tree Parsing Support

The library supports parsing device trees for:
- POWER devices: Fully supported for hardware running IBM POWER-based firmware.
- SPARC devices: Suitable for systems leveraging Sun Microsystems SPARC architecture.
- ARM devices: Provides efficient compatibility with ARM-based systems using device trees.

#### Example Use Cases
- **Pommed**: A hardware management tool for Apple laptops that integrates `libofapi`.
- **Embedded Systems**: Parsing and configuring firmware for IoT devices and ARM platforms.

#### Why Use `libofapi`?
- It mirrors Linux kernel's internal API, making it familiar to developers working with device trees.
- Ideal for cross-platform hardware configuration and analysis in user space.
- Lightweight and performant, ensuring efficient integration into your projects.

---

For more information or advanced usage tips, refer to the examples in the repository or contact the maintainers via GitHub Issues.
