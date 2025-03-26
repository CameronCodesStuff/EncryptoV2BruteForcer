# EncryptoV2 Brute Forcer

A powerful brute-force tool designed to test the security of AES-encrypted data from [EncryptoV2](https://cameroncodesstuff.github.io/EncryptoV2/). This tool systematically attempts various keys to decrypt AES-encrypted messages.

## ⚠️ Disclaimer
This project is intended for educational and security research purposes only. Unauthorized use of this tool against systems you do not own or have permission to test is illegal. Use responsibly.

## Features
- Multi-threaded brute force for maximum efficiency
- Customizable key length and charset options
- Supports dictionary and brute-force attacks
- Lightweight and easy to use

## Installation
Ensure you have Python installed, then clone the repository:

```sh
git clone https://github.com/yourusername/EncryptoV2-BruteForcer.git
cd EncryptoV2-BruteForcer
pip install -r requirements.txt
```

## Usage
Run the brute-forcer with the required parameters:

```sh
python brute_forcer.py --ciphertext "YOUR_CIPHERTEXT" --mode brute --charset abc123 --max-length 6
```

### Options:
- `--ciphertext` : The encrypted text to brute force
- `--mode` : Attack mode (`brute` for brute force, `dict` for dictionary attack)
- `--charset` : Characters to use in brute force
- `--max-length` : Maximum key length
- `--wordlist` : Path to a dictionary file (for dictionary attack mode)

## Example
Using a dictionary attack:

```sh
python brute_forcer.py --ciphertext "ENCRYPTEDTEXT" --mode dict --wordlist wordlist.txt
```

## Contributing
Pull requests are welcome! Feel free to submit issues or feature requests.

## License
MIT License. See `LICENSE` for details.

