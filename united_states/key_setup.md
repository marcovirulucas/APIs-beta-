To ensure security and avoid exposing your private keys in the code, follow these steps to set up your environment:
1. **Obtain your Key:**
Get your free API key from the [BLS Registration page](https://data.bls.gov/registrationEngine/).
2. **Create a `keys.py` file:** 
In your Google Colab file browser (or your local folder), create a file named `keys.py`.
3. **Add your key:** Inside `keys.py`, add the following line:
```python
bls_key = "YOUR_SECRET_KEY_HERE"
4. **Implementation:**
The scripts are designed to import this key securely
```python
import keys
# Fetching the key from the keys.py file
key = '{}'.format(keys.bls_key)
