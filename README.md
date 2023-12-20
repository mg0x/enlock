## 📜Enlock - File Encryption Tool

Enlock is a simple command-line file encryption tool written in Golang. It simplifies the generation RSA key pairs, the encryption and decryption of files using AES-256, and ensures secure file transmission.

### Features

    🔐 RSA Key Pair Generation: Generate a pair of strong RSA public and private keys for secure encryption and decryption.

    🌐 AES-256 Encryption: Encrypt files or directories using a randomly generated AES-256 key.

    🔑 Passphrase Protection: Protect your private key by encrypting it with a passphrase using Argon2i Key Derivation Function (KDF).

    📦 Secure File Transmission: Use the recipient's public key to encrypt the AES-256 key, ensuring secure file transmission.

### Generated Zip File

When you use Enlock to encrypt a file or directory, it creates a zip file that contains the following:

- Encrypted File/Directory: The content of the file or directory is encrypted using AES-256.

- AES Key File: A file containing the randomly generated AES-256 key used for encryption. This key is encrypted using the recipient's public key.

- Public Key File: The RSA public key of the recipient.

- Encrypted Private Key File: Your private key, encrypted with a AES-256 key generated from the user passphrase using Argon2i KDF.


### Installation

Download the latest release from the Releases page.

```sh
# Example installation
./install.sh
``` 


## Disclaimer

🚨 This software is provided without any guarantees or warranties. It is your responsibility to use it in compliance with applicable laws and regulations.

🤝 Contributions are welcome! Please follow our Contribution Guidelines for details.
License

📜 This project is licensed under the MIT License.