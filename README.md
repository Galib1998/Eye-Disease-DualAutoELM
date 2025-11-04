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
![t-SNE Plot] <img width="1820" height="489" alt="84539616-fb56-4407-9e57-a5d4bc007e00" src="https://github.com/user-attachments/assets/c5b35cc6-c60a-44b1-87f7-c9bd8c38b5ce" />

Generating reconstruction comparison for ConvAE 
<img width="1452" height="593" alt="9402bd3f-7fe0-4c80-aeda-d9794306690b" src="https://github.com/user-attachments/assets/d3f4539a-88f7-4885-b9a8-deea13ceabb3" />

Generating reconstruction comparison for VAE
<img width="1452" height="593" alt="6fb78167-c08c-4437-b5c5-abd9e22bbf88" src="https://github.com/user-attachments/assets/e6381609-41fd-43bf-b274-246ea20af698" />

Generated 5 input images with 3 attention maps each
<img width="1589" height="1973" alt="7e2e5062-63b0-49a8-93b9-ebdd5c4bccdc" src="https://github.com/user-attachments/assets/2eea65da-ff90-4d69-bf5a-ec4eea6e3ffb" />

Generating  Class-wise ROC Curves with Metrics
<img width="1990" height="1189" alt="30d719e2-9128-4771-b037-523d6d1d939d" src="https://github.com/user-attachments/assets/535bcb0e-04fd-49a0-99b3-dc4fb56c493d" />
