# show ja3 hashes in wireshark

A ja3 hash is a way of fingerprinting different TLS configurations made by looking at the key negotiation step. Different libraries use different crypto defaults and you can use the signatures to help spot unusual sources of encrypted traffic without needing to decrypt them.

First step is to add a couple of .lua files found from [this repo](https://github.com/fullylegit/ja3) to your plugins dir
(on my mac it's `~/.config/wireshark/plugins`)

Then when you restart wireshark, find a TLS handshake with `tls.handshake` and you should notice a new layer in the packet details window.
