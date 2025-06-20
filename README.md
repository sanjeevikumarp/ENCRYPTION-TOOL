# ENCRYPTION-TOOL

company:codtech it solutions

name:sanjeevi kumarp

intern id:CT04DF239

domain:cyber security&ethical hacking

duration:4weeks

mentor:neela santosh

output:

python aes_tool.py secret.txt secret.key

python aes_tool.py secret.txt.aes secret.key --decrypt


# AES File Encryptor/Decryptor

This Python script allows you to encrypt and decrypt files using AES (Advanced Encryption Standard) encryption with a randomly generated key. The key is stored in a separate file for security.

---

##  Disclaimer

> **Use this tool responsibly.** Encrypting or decrypting files you do not own or have permission to access may be illegal.

---

##  Features

- Encrypts any file using AES in EAX mode.
- Generates a secure random 16-byte key.
- Saves the key to a separate file.
- Deletes the original file after encryption.
- Supports decryption with verification using the same key.

---

##  Usage

###  Encrypt a File

```bash
python aes_tool.py myfile.txt keyfile.key
```

This will:
- Encrypt `myfile.txt` to `myfile.txt.aes`
- Store the key in `keyfile.key`
- Delete the original `myfile.txt`

###  Decrypt a File

```bash
python aes_tool.py myfile.txt.aes keyfile.key --decrypt
```

This will:
- Decrypt `myfile.txt.aes` using `keyfile.key`
- Output the original file `myfile.txt`

---

##  Arguments

| Argument         | Description                                              |
|------------------|----------------------------------------------------------|
| `file_path`      | Path to the file to encrypt or decrypt                   |
| `key_path`       | Path to save the generated key or read the key for decryption |
| `--decrypt`      | Optional flag to switch to decrypt mode (default is encrypt) |

---

##  Requirements

- Python 3.x
- `pycryptodome` package

Install it with:

```bash
pip install pycryptodome
```

---

##  Security Notes

- Always keep the key file safe and secure.
- Losing the key means losing access to the encrypted data.
- This script uses AES EAX mode which ensures confidentiality and integrity.

---

##  Example

```bash
python aes_tool.py secret.txt secret.key
python aes_tool.py secret.txt.aes secret.key --decrypt
```

---

## Author

Built for educational and secure file storage purposes.
