# QRTurn.com API Document

QRTurn.com is the WEB application for QR code scan or generation.

"QR Everywhere."

# USAGE

**redirectUrl**
- `redirectUrl` - This is the final destination where the QR data is delivered.

**data**
- `data` - This is the data that generates the QR code.

```
https://qrturn.com/scan?returnUrl=https://google.com
//For sell ​​with 12 Dogecoin (DOGE)

https://qrturn.com/scan?returnUrl=https://google.com
//For sell ​​with 12 Dogecoin (DOGE)

```

# INSTALLATION TO YOUR WEB
Include script on your site.

```
<script type="text/javascript" src="https://qrturn.com/qrturn.js"></script>
```

```
QRTurn.returnUrl = "https://google.com?param=data" // QR scan
QRTurn.scan()

QRTurn.data = "dogecoin:DN7WNoyLx6DRoQpuzpcLhV95vLARFdbZ9A?acmount=12" // QR generation
QRTurn.gen()
```

# LICENSE
[MPL-2.0](https://www.mozilla.org/MPL/2.0/)
