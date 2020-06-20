# Show any field in the packet list display

This can be done with any field but this example shows the full URL for HTTP requests.

In the display filter type `http.request` to show requests for web pages.

Scroll down the packet info window and make sure `Hypertext Transfer Protocol` is expanded. Then right click on the text that says `Full request URI:` and choose `Apply as Column`. Packets containing web requests should now have the full URL visible in the packet 

## Useful fields to display
depends on what protocol you're interested in obviously, but these are pretty handy

field | fieldname
----|---
Country* | `ip.geoip.country`
HTTP URL| `http.request.full_uri`
TLS server identifier| `ssl.handshake.extensions_server_name`
[JA3](ja3.md) signature| `ja3.hash`

\* requires you to manually [add a geoIP db](https://wiki.wireshark.org/HowToUseGeoIP) first.
