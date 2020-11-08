```bash
# Install some prerequisites needed by adding GPG public keys
$ sudo apt-get install gnupg ca-certificates curl

# Import our GPG key. Notice the hyphen at the end of line.
$ curl -sSL https://v2fly.org/debian/pubkey.gpg | sudo apt-key add -

# Add the our official APT repository:
$ echo "deb [arch=amd64] https://v2fly.org/debian/ $YOUR_DISTRIBUTION main" | sudo tee /etc/apt/sources.list.d/v2ray.list

# To update the APT index:
$ sudo apt-get update

# You can install V2Ray from APT now:
$ sudo apt-get install v2ray
```
