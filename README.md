
# RIFT: Multi-Modal Image Matching Based on Radiation-Variation Insensitive Feature Transform

RIFT is a Python implementation for multimodal image matching and rotation-invariant feature detection using phase congruency.


## Project Structure

```
RIFT-MULTIMODAL-MATCHING-PYTHON/
│
├── images/
│   ├── day-night/
│   ├── depth-optical/
│   ├── infrared-optical/
│   ├── map-optical/
│   ├── optical-optical/
│   ├── sar-optical/
│   └── thermal-optical-mp/
│
├── src/
│   ├── phase_congruency/
│   │   ├── phasecong.py
│   │   ├── tools.py
│   │   └── matcher_functions.py
│   └── RIFT2.py
│
├── demo.py
└── README.md
```

### Directories and Files

- **images/**: Contains various categories of image pairs used for multimodal matching.
- **src/**: Contains the source code for the project.
  - **phase_congruency/**: Module for phase congruency computation and related tools.
  - **RIFT2.py**: Main implementation of the RIFT2 feature detector and descriptor.
  - **matcher_functions.py**: Contains functions for feature matching and orientation calculation.
- **demo.py**: Demonstrates the usage of the RIFT2 implementation.

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/GaotTian/RIFT-Multimodal-matching-python.git
   cd RIFT-MULTIMODAL-MATCHING-PYTHON
   ```

2. Installation:

   **Option 1:** Create conda environment from the `environment.yml`:
   ```sh
   conda env create -f environment.yml
   conda activate rift2
   ```

  **Option 2:** Install the required packages using pip from the `requirements.txt` (Python 3.11 is recommended ):
   ```sh
   pip install -r requirements.txt
   ```

## Usage
Change the `image_path` and `image_name` variables in the `demo.py` file to the desired image pair. Then, run the following command to execute the demo:
```sh
python demo.py
```

## Credits
This Python implementation of RIFT is inspired by the author's original implementation in MATLAB: [RIFT MATLAB Implementation](https://github.com/LJY-RS/RIFT-multimodal-image-matching).

The Python implementation of phase congruency used in this project is adapted from: [PhasePack by alimuldal](https://github.com/alimuldal/phasepack/tree/master).
