# CFD
# OpenFOAM Simulation Projects

Welcome to the **OpenFOAM Simulation Projects** repository! This repository contains computational fluid dynamics (CFD) simulation projects created using OpenFOAM, a powerful open-source tool for solving fluid mechanics and heat transfer problems. The projects also utilize visualization tools like ParaView to present simulation results in a clear and interactive manner.

---

## Repository Structure

The repository is organized into the following directories:

```
|-- tutorials/
|   |-- incompressible/
|       |-- icoFoam/
|           |-- elbow_quad/
|           |-- elbow_tri/
|           |-- cavity/
|-- results/
|   |-- images/
|   |-- animations/
|-- scripts/
|-- README.md
```

### Key Directories:
- **`tutorials/`**: Contains simulation case files for OpenFOAM tutorials, including customizations and meshes like `elbow_quad` and `elbow_tri`.
- **`results/`**: Stores outputs, images, and animations generated from simulations.
- **`scripts/`**: Includes utility scripts for preprocessing, running simulations, and automating visualization.

---

## Projects Overview

### 1. **Elbow Flow Simulation**
   - **Description**: Simulates fluid flow through an elbow pipe using different mesh configurations (triangular and quadrilateral).
   - **Tools Used**: OpenFOAM (icoFoam solver) and ParaView.
   - **Files**:
     - `elbow_tri.msh`: Triangular mesh.
     - `elbow_quad.msh`: Quadrilateral mesh.
     - `constant/`, `system/`, and `0/` directories.

## Getting Started

### Prerequisites
1. Install **OpenFOAM**.
   - Verify the installation by running:
     ```bash
     foamVersion
     ```
2. Install **ParaView** for visualization.

### Running Simulations
1. Navigate to the desired tutorial directory (e.g., `elbow_tri`):
   ```bash
   cd tutorials/incompressible/icoFoam/elbow_tri
   ```
2. Run the preprocessor:
   ```bash
   fluentMeshToFoam elbow_tri.msh
   ```
3. Run the simulation:
   ```bash
   icoFoam
   ```
4. Visualize results in ParaView:
   ```bash
   paraview
   ```

---

## Visualization with ParaView

1. Open ParaView and load the case results.
2. Apply filters like streamlines, slices, and volume rendering for insights.
3. Compare results side-by-side (e.g., `elbow_quad` vs. `elbow_tri`).

---

## Future Work
- Expanding simulations to include transient and turbulent flows.
- Exploring custom solvers and advanced boundary conditions.
- Leveraging GPU acceleration for faster computation.

---

## Contributing
Contributions are welcome! If you have ideas for new simulations or enhancements, please fork this repository and submit a pull request.

---

## Contact
For any questions or discussions, feel free to reach out via the Issues tab or contact the repository maintainer at [avisingh0172@gmail.com].


