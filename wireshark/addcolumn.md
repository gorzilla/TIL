# Show any field in the packet list display

This can be done with any field but this example shows the full URL for HTTP requests.

In the display filter type `http.request` to show requests for web pages.

Scroll down the packet info window and make sure `Hypertext Transfer Protocol` is expanded. Then right click on the text that says `Full request URI:` and choose `Apply as Column`. Packets containing web requests should now have the full URL visible in the packet 

## Useful fields to display

Depends what protocol you're interested in obviously, but I find these handy

field | fieldname
----|---
Country* | `ip.geoip.country`
HTTP URL| `http.request.full_uri`
[JA3](ja3.md) signature**| `ja3.hash`
TLS server identifier***| `tls.handshake.extensions_server_name`

\* needs [a geoIP db](https://gitlab.com/wireshark/wireshark/-/wikis/HowToUseGeoIP)

\** needs a [plugin](https://github.com/fullylegit/ja3)

\*** if you haven't updated Wireshark recently it will be `ssl.handshake...` but that's deprecated and you should update.
