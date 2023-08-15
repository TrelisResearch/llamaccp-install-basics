## Mac Installation:
*for detailed instructions go to the [original repo](https://github.com/ggerganov/llama.cpp)

1. **Download the Code**:
    ```bash
    git clone https://github.com/ggerganov/llama.cpp && cd llama.cpp
    ```

2. **Standard Build**:
    ```bash
    make
    ```

3. **GPU Acceleration on Apple Devices**:
    ```bash
    LLAMA_METAL=1 make
    ```

> **Note for Mac with M1**: Simply prepend `LLAMA_M1=1` before any `make` command mentioned above.

## Windows Installation:
1. **Download the Code**:
    ```bash
    git clone https://github.com/ggerganov/llama.cpp && cd llama.cpp
    ```

2. **Setup and Build**:
    - Download and extract the latest `fortran` version of `w64devkit`.
    - Run `w64devkit.exe`.
    - Navigate to the `llama.cpp` directory.
    ```bash
    make
    ```

3. **BLAS Acceleration with OpenBLAS**:
    - Download `OpenBLAS` for Windows.
    - Copy necessary files from the `OpenBLAS` zip to the appropriate `w64devkit` directories.
    ```bash
    make LLAMA_OPENBLAS=1
    ```

> **Note**: This is a summarized version. For detailed instructions or troubleshooting, refer to the original documentation.
