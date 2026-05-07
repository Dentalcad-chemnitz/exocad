# exocad
Exocad DentalCAD repository featuring digital dental design workflows, models, and CAD/CAM chemnitz insights.
# Exocad DentalCAD Chemnitz

Welcome to the **Exocad DentalCAD Chemnitz** repository. This project is focused on digital dentistry workflows, CAD/CAM integration, and modern dental laboratory automation using Exocad DentalCAD technologies. The goal of this repository is to provide educational resources, workflow examples, and simple development utilities that support dental design environments.

This repository includes:

* Digital dental workflow concepts
* CAD/CAM process documentation
* Python automation examples
* Data organization examples for dental cases
* Basic scripting for workflow optimization

## Features

* Exocad workflow examples
* Dental case management scripts
* CAD file organization utilities
* Simple automation using Python
* Research and testing environment for digital dentistry

---

# Project Structure

```bash
exocad-dentalcad-chemnitz/
│
├── workflows/
├── scripts/
├── cases/
├── exports/
├── README.md
└── requirements.txt
```

---

# Python Example: Dental Case Management

The following Python script demonstrates a simple dental case management structure that can be expanded for laboratory workflows.

```python
class DentalCase:
    def __init__(self, patient_name, case_id, restoration_type):
        self.patient_name = patient_name
        self.case_id = case_id
        self.restoration_type = restoration_type

    def display_case(self):
        print(f"Patient: {self.patient_name}")
        print(f"Case ID: {self.case_id}")
        print(f"Restoration: {self.restoration_type}")


case1 = DentalCase(
    patient_name="John Doe",
    case_id="EXO-2026-001",
    restoration_type="Zirconia Crown"
)

case1.display_case()
```

---

# Workflow Automation Example

This example automatically creates folders for new dental cases.

```python
import os

def create_case_folder(case_id):
    folder_name = f"cases/{case_id}"

    if not os.path.exists(folder_name):
        os.makedirs(folder_name)
        print(f"Folder created: {folder_name}")
    else:
        print("Case folder already exists")

create_case_folder("EXO-2026-001")
```

---

# Digital Dentistry Workflow

Typical workflow used in this repository:

1. Intraoral scanning
2. STL data preparation
3. Exocad DentalCAD modeling
4. Margin line adjustment
5. Restoration design
6. Export to CAM software
7. Milling or 3D printing
8. Final finishing and quality control

---

# Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/exocad-dentalcad-chemnitz.git
```

Install required packages:

```bash
pip install -r requirements.txt
```

---

# Requirements

```txt
Python 3.10+
numpy
pandas
opencv-python
```

---

# Future Development

Planned improvements include:

* STL file validation tools
* Automated case tracking
* AI-assisted dental workflow analysis
* Dental restoration reporting
* Exocad export optimization scripts

---

# Disclaimer

This repository is intended for educational and research purposes only. It is not officially affiliated with Exocad GmbH. Users should follow professional dental laboratory standards and local regulations when implementing production workflows.

---

# Contribution

Contributions are welcome. Feel free to submit pull requests, workflow ideas, automation scripts, or documentation improvements related to digital dentistry and CAD/CAM systems.

---

# License

This project is distributed under the MIT License.
