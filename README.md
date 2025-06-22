🖋️ Handwritten Digit Generator Web App (MNIST × VAE)
This is a Streamlit-based web application that generates handwritten digit images (0–9) using a Variational Autoencoder (VAE) trained on the MNIST dataset.

Users can interact with the app via a clean interface and generate five synthetic digit images with a single click. The generated images follow the style and shape distribution of real handwritten digits.

🧠 Features
✅ Generates 5 unique images of digits each time

✅ Built using PyTorch and Streamlit

✅ Trained on MNIST (28×28 grayscale images)

✅ Publicly accessible for anyone to try

✅ Deployable via Streamlit Cloud

📸 Demo
![Demo GIF or Screenshot Placeholder]

(You can replace this with a screenshot or a short GIF after deployment.)

🧱 How It Works
1. Model Architecture
The core of this app is a Variational Autoencoder (VAE) with:

Encoder: Compresses 28×28 digit images to a latent space of 20 dimensions

Decoder: Reconstructs images from latent space

Sampling: Uses the reparameterization trick to generate diverse digits

2. Training
Dataset: MNIST (grayscale images of digits 0–9)

Platform: Trained using Google Colab on T4 GPU

Loss: Binary Cross Entropy + KL Divergence

Output: Trained model saved as vae_mnist.pth

3. Web Application
Framework: Streamlit

Input: Button click (no digit selection in current version)

Output: Five 28×28 generated handwritten digits displayed using Matplotlib

🗂️ File Structure
graphql
Copy
Edit
├── app.py              # Streamlit app code
├── vae_mnist.pth       # Trained VAE model weights
└── requirements.txt    # Dependencies for running the app
🚀 How to Run Locally
bash
Copy
Edit
# Clone the repository
git clone https://github.com/your-username/mnist-digit-generator.git
cd mnist-digit-generator

# Install dependencies
pip install -r requirements.txt

# Run the Streamlit app
streamlit run app.py
🌐 Live Demo
👉 Try the app here: https://your-username.streamlit.app

Note: It may sleep when inactive; wait a few seconds to load.

📦 Requirements
Python 3.7+
streamlit
torch
matplotlib

✍️ Author
Hafsa Naz
🔗 LinkedIn
www.linkedin.com/in/hafsa-naz

📜 License
This project is licensed under the MIT License – see the LICENSE file for details.

