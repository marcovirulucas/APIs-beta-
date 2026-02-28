To ensure security and avoid exposing my private key in the code, I store it in a separate file named `keys.py`. Follow these steps to set up your key in the environment.

1. **Obtain your Key.**
Get your free API key from the website of the institution. In the case of the Bureau of Labor Statistics, visit [BLS Registration page](https://data.bls.gov/registrationEngine/).
2. **Create a separate file.** 
In your Google Colab file browser (or your local folder), create a file named `keys.py`.
3. **Add your key.** Inside `keys.py`, add the following line:
```python
bls_key = "YOUR_SECRET_KEY_HERE"
```
4. **Implementation.**
The scripts are designed to import this key securely
```python
import keys
# Fetching the key from the keys.py file
key = '{}'.format(keys.bls_key)
