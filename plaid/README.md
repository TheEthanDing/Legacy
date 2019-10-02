### plaid-python quickstart

[Quickstart guide](https://plaid.com/docs/quickstart)

``` bash
git clone https://github.com/plaid/quickstart.git
cd quickstart/python

# If you use virtualenv
# virtualenv venv
# source venv/bin/activate

pip install -r requirements.txt

# Start the Quickstart with your API keys from the Dashboard
# https://dashboard.plaid.com/account/keys
#
# PLAID_PRODUCTS is a comma-separated list of products to use when initializing
# Link. Note that this list must contain 'assets' in order for the app to be
# able to create and retrieve asset reports.
PLAID_CLIENT_ID='5d94b2f952cdf50014df5cf2' \
PLAID_SECRET='81ccdae4caa61aad22d06b6c0f1ebd' \
PLAID_PUBLIC_KEY='4baffeae021f610d71836fafbecfff' \
PLAID_ENV='sandbox' \
PLAID_PRODUCTS='transactions' \
PLAID_COUNTRY_CODES='US,CA,GB,FR,ES' \
python server.py
# Go to http://localhost:5000
```
