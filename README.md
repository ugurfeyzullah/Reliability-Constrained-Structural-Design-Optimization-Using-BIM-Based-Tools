# Reliability-Constrained Structural Design Optimization Using BIM-Based Tools

![Frame FORM](https://github.com/user-attachments/assets/9ebc2b38-acc3-43ac-b416-9d6a01969f5d)


**Quick Links:** [Documentation](#features) / [Installation](#installation) / [Usage](#usage) / [Paper](https://www.preprints.org/manuscript/202404.0060/v1) /  [Citation](#citation) / [Contact](#contact)

This project focuses on reliability-constrained structural design optimization by integrating Building Information Modeling (BIM) tools with artificial intelligence (AI) techniques. It aims to achieve a safe, economical, and sustainable design while handling real-world uncertainties in material properties and loads.

The project was conceptualized and performed during the research stay at the research group of Jun.-Prof. Dr. Reza Maalek, the GOLDBECK endowed chair in Digital Engineering and Construction (DEC) at the Institute of Technology and Management in Construction (TMB) of the Karlsruhe Institute of Technology (KIT). The findings and experimental details were published in "journal will be added". The author contributions are as follows:

Conceptualization, R.M. and F.Y.; methodology, R.M., F.Y.; software, F.Y.; validation, F.Y.; formal analysis, F.Y.; investigation, R.M. and F.Y.; resources, R.M.; data curation, F.Y.; writing—original draft preparation, F.Y.; writing—review and editing, R.M.; visualization, F.Y.; supervision, R.M.; project administration, R.M.; funding acquisition, R.M.






https://github.com/ugurfeyzullah/Intelligent-Optimization-of-Steel-Structures-Through-Bim-Based-Visual-Programming-Platform-and-Tools/assets/149387821/1261d706-0fb2-452e-8fc2-2f25243358e3





## Features

- **Structural and Reliability Analysis:** Combines Finite Element Method (FEM) with First Order Reliability Method (FORM).
- **Metaheuristic Optimization:** Employs Differential Evolution (DE) for solving complex design optimization problems under reliability constraints.
- **BIM Integration:** Utilizes Dynamo, Revit, and Robot Structural Analysis (RSA) for parametric modeling and optimization.
- **Python Libraries:** PyNiteFEA for FEM analysis, PyMoo for optimization, and PyStra for stochastic reliability assessment.
- 
## Methodology

The workflow encompasses these main phases:
1.	Create parametric trusses by using VP ;
2.	Create a FEM model to perform structural analyses;
3.	Perform reliability analysis;
4.	Change the design variables with MA and perform multiple reliability analysis until design criteria are fulfilled;
5.	Import optimized model to the BIM environment for further adjustments.

   ![Comprehensive workflow of the VP -Based RBDO methodology](https://github.com/user-attachments/assets/ca3fa8cb-f302-40fe-804b-a5e95351fc44)



## Getting Started

### Prerequisites

- **Dynamo** (v3.0.4) for visual programming.
- **PyNiteFEA** (v0.0.94) for structural analysis.
- **PyMoo** (v0.6.1) for multi-objective optimization.
- **PyStra** (v1.3.0) for reliability analysis.

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/ugurfeyzullah/Reliability-Constrained-Structural-Design-Optimization-Using-BIM-Based-Tools.git
    ```
2. Install necessary dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the optimization script on Dynamo:


## Usage

1. **Model Setup**: Create parametric structural models in Dynamo by defining node coordinates and connecting elements using a visual scripting approach.
2. **Define Inputs**: Set design variables, including cross-sectional areas and nodal coordinates, in Dynamo. Adjust boundary conditions and material properties.
3. **Structural Analysis**: Run Finite Element Analysis (FEM) using PyNite within the Dynamo environment to compute stress, displacement, and reliability metrics.
4. **Optimization**: Use Differential Evolution (DE) from the PyMoo library to optimize design variables under reliability constraints.
5. **Reliability Check**: Perform reliability analysis using the First-Order Reliability Method (FORM) with PyStra to calculate reliability indices and evaluate uncertainty in loads and material properties.
6. **Model Integration**: Import optimized models to Autodesk Robot Structural Analysis (RSA) for further structural adjustments or analysis, then transfer the model back to Revit for final design adjustments.
7. **Evaluation**: Assess the optimization and reliability results, ensuring the design satisfies safety, reliability, and cost-effectiveness criteria.
8. **Data Handling**: Use custom Python functions to pull AISC section properties from Excel for batch analysis and structural simulations.




## Contributing

Contributions are welcome! If you have improvements or bug fixes, please follow these steps:

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -am 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a pull request.

## Citation (To be updated)

MDPI and ACS Style
Yavan, F.; Maalek, R.; Toğan, V. Structural Optimization of Trusses in Building Information Modeling (BIM) Projects Using Visual Programming, Evolutionary Algorithms, and Life Cycle Assessment (LCA) Tools. Buildings 2024, 14, 1532. https://doi.org/10.3390/buildings14061532

AMA Style
Yavan F, Maalek R, Toğan V. Structural Optimization of Trusses in Building Information Modeling (BIM) Projects Using Visual Programming, Evolutionary Algorithms, and Life Cycle Assessment (LCA) Tools. Buildings. 2024; 14(6):1532. https://doi.org/10.3390/buildings14061532

Chicago/Turabian Style
Yavan, Feyzullah, Reza Maalek, and Vedat Toğan. 2024. "Structural Optimization of Trusses in Building Information Modeling (BIM) Projects Using Visual Programming, Evolutionary Algorithms, and Life Cycle Assessment (LCA) Tools" Buildings 14, no. 6: 1532. https://doi.org/10.3390/buildings14061532

BibTex:

@Article{buildings14061532,
AUTHOR = {Yavan, Feyzullah and Maalek, Reza and Toğan, Vedat},
TITLE = {Structural Optimization of Trusses in Building Information Modeling (BIM) Projects Using Visual Programming, Evolutionary Algorithms, and Life Cycle Assessment (LCA) Tools},
JOURNAL = {Buildings},
VOLUME = {14},
YEAR = {2024},
NUMBER = {6},
ARTICLE-NUMBER = {1532},
URL = {https://www.mdpi.com/2075-5309/14/6/1532},
ISSN = {2075-5309},
DOI = {10.3390/buildings14061532}
}

## Contact

- Feyzullah YAVAN - www.linkedin.com/in/ugurfey - feyzullah.yavan@kit.edu


## License

This project is licensed under the Apache License - see the [LICENSE](LICENSE.md) file for details.
