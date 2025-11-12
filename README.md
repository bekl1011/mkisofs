## 📜 Licensing and Source Code Information

This repository contains binary executables and dynamic link libraries (DLLs) distributed under various free and open-source licenses. To comply with the terms of these licenses, the complete corresponding source code for all included binaries is provided in the `/sourceCode` directory.

---

### 📝 Component Breakdown and Licensing

The following table lists the included binary files and the license that governs their use and redistribution.

| Binary File | Function / Source Package | License |
| :--- | :--- | :--- |
| `mkisofs.exe` | The main application program (from `cdrtools`) | **GNU General Public License (GPL)** |
| `cygwin1.dll` | The Cygwin runtime compatibility layer | **GNU Lesser General Public License (LGPLv3 or later) with a linking exception** |
| `cygiconv-2.dll` | Character Set Conversion Library (from `libiconv`) | **GNU Lesser General Public License (LGPL)** |
| `cygintl-8.dll` | Internationalization Library (from `gettext`) | **GNU Lesser General Public License (LGPL)** |

---

### 📖 Required License Texts

Copies of the full text for the required licenses are included in the repository root:

* **`LICENSE-GPL.txt`**: The full text of the GNU General Public License (for `mkisofs.exe`).
* **`LICENSE-LGPL.txt`**: The full text of the GNU Lesser General Public License (for the DLLs).
* **`LGPL-CYGWIN-EXCEPTION.txt`**: The text detailing the linking exception for `cygwin1.dll`.

---

### 📦 Source Code Access

In compliance with the GPL and LGPL, the complete, corresponding source code for the binaries included in this repository is available in the **`/sourceCode`** directory.

The directory contains the original source code archives (e.g., `.tar.gz`) for the following projects, matching the binaries included in this release:

* **`cdrtools-3.0.0.tar`** (Source for `mkisofs`)
* **`newlib-cygwin-1_7_6.tar`** (Source for `cygwin1.dll`)
* **`libiconv-1.13.1.tar`** (Source for `cygiconv-2.dll`)
* **`gettext-0.18.1.1.tar`** (Source for `cygintl-8.dll`)

**⚠️ Note on Large Files (Git LFS Required)**

Due to the size of some essential source archives (specifically, `cygwin-1_7_6.tar` and `gettext-0.18.1.1.tar`), this repository uses **Git Large File Storage (Git LFS)**.

To successfully clone this repository and download the large source archives, you **must** install Git LFS before cloning.

#### Cloning Instructions:

1.  **Install Git LFS:**
    ```bash
    # On Debian/Ubuntu
    sudo apt-get install git-lfs 
    # Or, on macOS using Homebrew
    brew install git-lfs 
    # Or, download from git-lfs.com 
    ```

2.  **Initialize LFS:**
    ```bash
    git lfs install
    ```

3.  **Clone the repository (Standard Clone):**
    ```bash
    git clone [https://github.com/bekl1011/mkisofs.git](https://github.com/bekl1011/mkisofs.git)
    ```
    *(If you cloned before installing LFS, you may need to run `git lfs pull` after initialization to download the large files.)*
