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

1. **Parametric Truss Modeling** using Dynamo.
2. **FEM and Reliability Analysis** using Python and PyNiteFEA.
3. **Optimization** using metaheuristic algorithms (DE) integrated with the PyMoo library.
4. **Seamless Transfer to BIM** environments like Revit and RSA for further structural evaluation.





## Getting Started

### Prerequisites

- **Dynamo** (v3.0.4) for visual programming.
- **PyNiteFEA** (v0.0.94) for structural analysis.
- **PyMoo** (v0.6.1) for multi-objective optimization.
- **PyStra** (v1.3.0) for reliability analysis.

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/repository-name.git
    ```
2. Install necessary dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the optimization model:
    ```bash
    python optimize_model.py
    ```

## Usage

1. **Model Preparation**: Start by preparing your parametric structural model in Dynamo.
2. **Core node creation**: Create a core node from your parametric model by turning it into a custom node.
3. **Optimization with Dynamo**: Open the provided Dynamo script to perform optimization. Adjust input parameters as needed for your specific structural design requirements and change the provided core node if needed.
4. **Analysis in RSA**: Provided script will use RSA for detailed FEA as part of the optimization loop.
5. **Evaluation**: Evaluate the optimization results, including stress, displacement, and weight.
6. **Next generation creation**: Generate next generation by using metaheuristic algorithms. Python libraries or own generated python codes can be employed for this step. A sample code has been provided along with shared scripts.[Example Document](Optimization)
7. **Revit interaction**: Optimized design can be imported Revit for further analyses by using provided optimization script. [Example Document](<Optimization with Revit integration>)
8. **LCA and Cost Analysis**: Utilize Revit and Tally for environmental and economic assessment as presented in upcoming video.






## Contributing

Contributions are welcome! If you have improvements or bug fixes, please follow these steps:

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -am 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a pull request.

## Citation

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
