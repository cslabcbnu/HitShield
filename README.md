## HitShield:Enhanced swap eviction scheme for Multi-Generational LRU

- This repository contains the source code for the **HitShield (built in Linux kernel 6.8)** used in the research paper titled "**HitShield:Enhanced swap eviction scheme for Multi-Generational LRU**".
- The code implements new eviction scheme for Multi-Generational LRU. 
- This repository is provided to enable reproducibility and further research based on our work.

## Related Publication

*   **HitShield:Enhanced swap eviction scheme for Multi-Generational LRU**
    *   Authors: Minwoo Jo, Binwon Song, Hayong Jeong, Heeseung Jo
    *   Journal/Conference: IEEE Access
    *   Publication Date: 2025. 4.17.
    *   Link to Paper: https://doi.org/10.1109/ACCESS.2025.3558527

## Installation

To set up the environment and build the code, please follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/cslabcbnu/HitShield
    cd HitShield
    ```

2.  **Dependencies:**
    ```bash
    apt install -y build-essential bc libncurses5-dev bin86 libssl-dev bison flex libelf-dev
    ```

3.  **Build Instructions:**
    ```bash
    make O=~/build/kernel -j $(nproc)
    su -c 'make O=~/build/kernel INSTALL_MOD_STRIP=1 modules_install -j $(nproc) && make O=~/build/kernel install -j $(nproc) '
    ```

## Contact

If you have any questions, feel free to open an issue on this repository or contact hyeonsa@cbnu.ac.kr.

---

