# Reliability-Constrained Structural Design Optimization Using BIM-Based Tools

![Frame FORM](https://github.com/user-attachments/assets/9ebc2b38-acc3-43ac-b416-9d6a01969f5d)




https://github.com/user-attachments/assets/b18f9838-1d82-4e33-b570-3ac2a32dde9f





**Quick Links:** [Documentation](#features) / [Installation](#installation) / [Usage](#usage) / [Paper](https://www.preprints.org/manuscript/202404.0060/v1) /  [Citation](#citation) / [Contact](#contact)

This project focuses on reliability-constrained structural design optimization by integrating Building Information Modeling (BIM) tools with artificial intelligence (AI) techniques. It aims to achieve a safe, economical, and sustainable design while handling real-world uncertainties in material properties and loads.

The project was conceptualized and performed during the research stay at the research group of Jun.-Prof. Dr. Reza Maalek, the GOLDBECK endowed chair in Digital Engineering and Construction (DEC) at the Institute of Technology and Management in Construction (TMB) of the Karlsruhe Institute of Technology (KIT). The findings and experimental details were published in "journal will be added". The author contributions are as follows:

Conceptualization, R.M. and F.Y.; methodology, R.M., F.Y.; software, F.Y.; validation, F.Y.; formal analysis, F.Y.; investigation, R.M. and F.Y.; resources, R.M.; data curation, F.Y.; writing—original draft preparation, F.Y.; writing—review and editing, R.M.; visualization, F.Y.; supervision, R.M.; project administration, R.M.; funding acquisition, R.M.





https://github.com/user-attachments/assets/736bcc0a-e529-4b28-b4a9-1628cf33e4ca







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

## Citation 

MDPI and ACS Style
Yavan, F.; Maalek, R. Reliability-Constrained Structural Design Optimization Using Visual Programming in Building Information Modeling (BIM) Projects. Appl. Sci. 2025, 15, 1025. https://doi.org/10.3390/app15031025

AMA Style
Yavan F, Maalek R. Reliability-Constrained Structural Design Optimization Using Visual Programming in Building Information Modeling (BIM) Projects. Applied Sciences. 2025; 15(3):1025. https://doi.org/10.3390/app15031025

Chicago/Turabian Style
Yavan, Feyzullah, and Reza Maalek. 2025. "Reliability-Constrained Structural Design Optimization Using Visual Programming in Building Information Modeling (BIM) Projects" Applied Sciences 15, no. 3: 1025. https://doi.org/10.3390/app15031025

APA Style
Yavan, F., & Maalek, R. (2025). Reliability-Constrained Structural Design Optimization Using Visual Programming in Building Information Modeling (BIM) Projects. Applied Sciences, 15(3), 1025. https://doi.org/10.3390/app15031025

## Contact

- Feyzullah YAVAN - www.linkedin.com/in/ugurfey - feyzullah.yavan@kit.edu


## License

This project is licensed under the Apache License - see the [LICENSE](LICENSE.md) file for details.
