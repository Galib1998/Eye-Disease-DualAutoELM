# Eye Disease Detection using a CBAM-Guided Dual Autoencoder and ELM

This project implements a novel deep learning approach for detecting eye diseases from fundus images. The core of this project is a **Dual Autoencoder** (combining a Convolutional Autoencoder and a Variational Autoencoder) guided by a **Convolutional Block Attention Module (CBAM)** to extract highly representative features.

These features are then classified using an **Extreme Learning Machine (ELM)**, and the results are compared against other classifiers like MLPs. The `Eye-Disease-DualAutoELM.ipynb` notebook specifically visualizes the quality of these extracted features.

## Key Components
* **Dual Autoencoder (DAE):** A ConvAE and VAE work in parallel to capture both deterministic and probabilistic feature representations.
* **CBAM:** An attention mechanism that helps the autoencoders focus on the most salient regions of the images.
* **ELM:** A high-speed, single-hidden-layer feedforward network used for final classification.
* **t-SNE Visualization:** Used to visually confirm the feature separation and clustering quality.

## 🚀 How to Run this Project

1.  **Clone Repository**
    ```bash
    git clone (https://github.com/Galib1998/Eye-Disease-DualAutoELM.git)
    cd Eye-Disease-DualAutoELM
    ```

2.  **Install Dependencies**
    It is recommended to use a virtual environment.
    ```bash
    pip install -r requirements.txt
    ```

3.  **Add Data**
    This project requires the pre-extracted features from the autoencoders.
    * Place your feature files (e.g., `Eye-Disease-DualAutoELM.ipynb`) inside the `/data/` folder.

4.  **Run Notebooks**
    Launch Jupyter and navigate to the `/notebooks/` directory to run the analysis.
    ```bash
    jupyter notebook
    ```

## 📊 Results

The t-SNE visualization demonstrates the separation capabilities of the different feature sets (ConvAE, VAE, and Dual-Auto).

*(Add your t-SNE plot, confusion matrix, or accuracy table here)*

![t-SNE Plot](path/to/your/plot_image.png)