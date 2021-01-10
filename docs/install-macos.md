## Installation on macOS

1. [Download Bitcoin Core](https://bitcoin.org/en/download) and install it. 
   You might want to read the [full node guide](https://bitcoin.org/en/full-node). If
   you're serious, be sure to validate the signatures of what you download. This is the
   only way to know if you're running the Bitcoin that you expect.
1. Start Bitcoin. It will begin syncing.
1. Open the Preferences in Bitcoin Core (`⌘+,`).  
![prefs](/docs/img/01-prefs.png)
1. Edit the configuration file  
![conf](/docs/img/02-open-config.png)
1. Insert the lines
    ```
    server=1
    ```
    to enable the RPC server - this is how coldcore will communicate with Bitcoin Core.
    ![edit](/docs/img/03-conf.png)

    *Note:* if you're testing, you can also insert the line
    ```
    testnet=1
    ```
1. Restart Bitcoin for the new configuration to take effect.
