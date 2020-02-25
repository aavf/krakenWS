# Virtual enviroment
## Install and activate
In a terminal, from project folder:

```
python3 -m venv venv

. venv/bin/activate

# install websocket library

pip install websocket_client
```

## Config
### Make the krakenapi.py file executable.
You can use the "chmod 755" command (change mode). For example:

```
chmod 755 krakenws.py
```

### API keys
Copy/paste your API public key from account management into file called "API_Public_Key".

Copy/paste your API private (secret) key into file called "API_Private_Key".

An API key is only needed if you plan to use the private API endpoints to access your Kraken account (such as balance inquiries, placing/cancelling orders, account history exports, etc).

# Usage: ./krakenws feed [symbols]

Example: ./krakenws.py trade XBT/USD

Example: ./krakenws.py ticker XLM/USD XDG/XBT

Example: ./krakenws.py book ETH/USD DASH/USD REP/EUR

Example: ./krakenws.py openOrders

Example: ./krakenws.py ownTrades
