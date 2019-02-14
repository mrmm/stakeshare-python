# Description
This library is the Python client for [StakeShare](https://staking.live) node RPC Client

# Usage
## Create the client instance
You need to have your node up and running with a config file that have.
**Note: To make sur all transactio nrelated methods works fine you need to run
the daemon `-txindex=1`.**

```ini
rpcuser=<RPC_USERNAME>
rpcpass=<RPC_PASSWORD>
rpcport=5516
```

```python
from client import StakeShareClient
import json
import sys

client = StakeShareClient(
    user="<RPC_USERNAME>",
    password="<RPC_PASSWORD>",
    host="http://localhost:5516"
)
```

## Example
This method will get the balance of all your accounts:
```python
balance = client.get_balance("*")
print("Current balance of all accounts is : %s" % ())
```

# List of methods
Coming soon
