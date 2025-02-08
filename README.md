# Chaos-Based Image Encryption and Decryption

## 📌 Overview
This project implements **image encryption and decryption** using a **chaos-based algorithm**. Chaos theory is widely used in cryptography due to its sensitivity to initial conditions, which makes it highly secure for encryption. The algorithm uses chaotic maps to transform an image into an unrecognizable format and then decrypts it back to its original form.

## 🚀 Features
- **Encryption:** Converts the input image into an encrypted format using a chaotic system.
- **Decryption:** Restores the original image using the correct decryption key.
- **Security:** High randomness ensures strong encryption against attacks.
- **Lightweight:** Efficient implementation with minimal computational overhead.
- **Supports multiple formats:** Works with PNG, JPG, etc.

## 🛠️ Technologies Used
- **Python**
- **NumPy**
- **OpenCV**
- **Matplotlib**
- **Chaotic Maps (Logistic, Henon, Lorenz, etc.)**

## 📜 Algorithm Steps
1. **Preprocessing:** Read the image and convert it into pixel values.
2. **Chaotic Key Generation:** Generate keys using a chaotic map.
3. **Permutation:** Shuffle pixel positions based on chaos sequences.
4. **Diffusion:** Modify pixel values using XOR operations with chaotic keys.
5. **Decryption:** Reverse the diffusion and permutation steps using the same chaotic sequence.

## 📸 Example Usage 
### 🔑 Encryption
from chaos_encryption import encrypt_image

encrypt_image("input.jpg", "encrypted.png", key=0.1234)

## 🔓 Decryption
from chaos_encryption import decrypt_image

decrypt_image("encrypted.png", "decrypted.jpg", key=0.1234)

## 📥 Installation
## Clone the repository:
git clone https://github.com/yourusername/chaos-image-encryption.git
cd chaos-image-encryption

## Install dependencies:
pip install -r requirements.txt

## 📝 Notes
1.The key must be kept secret; without it, decryption is impossible.
2.Small changes in the key result in entirely different outputs.
3.Different chaotic maps can be tested for varying security levels.

## 📜 References
Chaos-Based Cryptography
Logistic Map in Cryptography

