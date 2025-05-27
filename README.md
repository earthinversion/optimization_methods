# Optimization Methods

This repository contains implementations of optimization algorithms commonly used in inverse problems and machine learning. Each algorithm is demonstrated through Jupyter notebooks with practical examples and visualizations.

## Contents

This workspace includes three optimization methods:

1. **Gradient Descent** (`gradient_descent.ipynb`)
   - Basic gradient descent for solving linear inverse problems

2. **Newton's Method** (`newtons_method.ipynb`) 
   - Second-order optimization using Hessian information

3. **Conjugate Gradient Method** (`conjugate_gradient_method.ipynb`)
   - Efficient method for solving linear systems

4. **BFGS** (Coming soon)
   - Quasi-Newton method for optimization

5. **Adaptive Methods** (Coming soon)
   - Adam Optimizer
   - L-BFGS
   - Trust Region Newton

6. **Stochastic Methods** (Coming soon)
   - Stochastic Gradient Descent (SGD)
   - Mini-batch Gradient Descent 
   - Genetic Algorithm
   - Simulated Annealing


## 🛠️ Environment Setup

### Prerequisites

- [Miniconda](https://docs.conda.io/en/latest/miniconda.html) or [Anaconda](https://www.anaconda.com/products/distribution)
- Git (optional, for cloning the repository)

### Installation

1. **Clone or download this repository** (if you haven't already):
   ```bash
   git clone https://github.com/earthinversion/optimization_methods.git
   cd optimization_methods
   ```

2. **Create the conda environment** from the provided `environment.yml` file:
   ```bash
   conda env create -f environment.yml
   ```

3. **Activate the environment**:
   ```bash
   conda activate optm
   ```

4. **Verify the installation** by starting Jupyter:
   ```bash
   jupyter lab
   ```
   or
   ```bash
   jupyter notebook
   ```

## 🚀 Running the Notebooks

### Option 1: Using Jupyter Lab (Recommended)

1. **Activate the environment**:
   ```bash
   conda activate optm
   ```

2. **Start Jupyter Lab**:
   ```bash
   jupyter lab
   ```

3. **Open any of the three notebooks**:
   - `gradient_descent.ipynb`
   - `newtons_method.ipynb`
   - `conjugate_gradient_method.ipynb`

4. **Run the cells** by pressing `Shift + Enter` or using the "Run" button in the toolbar.

### Option 2: Using Jupyter Notebook

1. **Activate the environment**:
   ```bash
   conda activate optm
   ```

2. **Start Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

3. **Navigate to and open** any of the three `.ipynb` files.

4. **Execute the cells** sequentially to see the optimization algorithms in action.

## Notebook Descriptions

### 1. Gradient Descent (`gradient_descent.ipynb`)

This notebook demonstrates the basic gradient descent algorithm for solving linear inverse problems of the form `min ||Gm - d||²`.

**Key Features:**
- Implementation of basic gradient descent with configurable learning rate
- Example using synthetic travel time tomography data
- Convergence analysis and visualization
- Model parameter evolution tracking

**Learning Objectives:**
- Understand the gradient descent update rule
- Learn about learning rate selection
- Visualize convergence behavior
- Apply to geophysical inverse problems

### 2. Newton's Method (`newtons_method.ipynb`)

This notebook implements Newton's method, which uses second-order derivative information (Hessian) for faster convergence.

**Key Features:**
- Full Newton's method implementation
- Comparison with gradient descent
- Quadratic convergence demonstration
- Handling of the Hessian matrix

**Learning Objectives:**
- Understand second-order optimization methods
- Learn about the trade-offs between computation and convergence speed
- Explore the role of the Hessian matrix
- Compare convergence rates with first-order methods

### 3. Conjugate Gradient Method (`conjugate_gradient_method.ipynb`)

This notebook presents the conjugate gradient method, an efficient algorithm for solving large linear systems.

**Key Features:**
- Conjugate gradient algorithm implementation
- Efficient solution of linear systems
- Comparison with direct methods
- Memory-efficient optimization

**Learning Objectives:**
- Understand conjugate directions and their properties
- Learn about Krylov subspace methods
- Explore efficient algorithms for large-scale problems
- Apply to systems where direct inversion is impractical

## 🔧 Dependencies

The environment includes the following key packages:

- **Python 3.11** - Programming language
- **Jupyter** - Interactive notebook environment
- **NumPy** - Numerical computing
- **Matplotlib** - Plotting and visualization
- **SciPy** - Scientific computing (if needed for advanced features)

All dependencies are specified in the `environment.yml` file and will be automatically installed when creating the conda environment.

## 📊 Expected Outputs

Each notebook will generate:

- **Convergence plots** showing how the objective function decreases over iterations
- **Parameter evolution plots** tracking how model parameters change during optimization
- **Comparison plots** (where applicable) showing differences between methods
- **Numerical results** including final parameter estimates and convergence statistics

## 🔍 Troubleshooting

### Common Issues

1. **Environment activation fails**:
   ```bash
   # Make sure conda is properly installed and initialized
   conda init
   # Restart your terminal and try again
   ```

2. **Jupyter doesn't start**:
   ```bash
   # Ensure the environment is activated
   conda activate optm
   # Try installing jupyter explicitly
   conda install jupyter
   ```

3. **Import errors in notebooks**:
   - Make sure you're running the notebooks in the correct environment (`optm`)
   - Check that all packages are installed: `conda list`

4. **Plots don't display**:
   - Ensure matplotlib backend is properly configured
   - Try restarting the Jupyter kernel

### Getting Help

If you encounter issues:

1. Check that the conda environment is properly activated
2. Verify all dependencies are installed: `conda list`
3. Try restarting Jupyter and re-running the notebooks
4. Check the Jupyter console for error messages

## 🎯 Learning Path

**Recommended order for studying the notebooks:**

1. **Start with Gradient Descent** - Understand the fundamental concepts
2. **Move to Newton's Method** - Learn about second-order methods
3. **Finish with Conjugate Gradient** - Explore efficient large-scale methods

Each notebook builds upon concepts from the previous ones, so following this order will provide the best learning experience.

## 📝 Notes

- All algorithms are implemented from scratch for educational purposes
- The examples use synthetic data to clearly demonstrate the optimization behavior
- Each notebook includes detailed comments explaining the mathematical concepts
- Visualizations are provided to help understand the convergence properties


