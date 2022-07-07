# dayyoung.github.io/qrturn API Document

dayyoung.github.io/qrturn is the WEB application for QR code scan or generation.

"QR Everywhere."

# USAGE

**redirectUrl**
- `redirectUrl` - This is the final destination where the QR data is delivered.

**data**
- `data` - This is the data that generates by QR code.

```
https://dayyoung.github.io/qrturn/scan?returnUrl=https://google.com
//Scan QR code and receive data into returnUrl.

https://dayyoung.github.io/qrturn/gen?data=dogecoin:DN7WNoyLx6DRoQpuzpcLhV95vLARFdbZ9A?amount=12
//Generation QR code For sell ​​with 12 Dogecoin.

```

# INSTALLATION TO YOUR WEB
Include script on your site.

```
<script type="text/javascript" src="https://dayyoung.github.io/qrturn/qrturn.js"></script>
```

```
QRTurn.returnUrl = "https://google.com?param=data" // QR scan
QRTurn.scan()

QRTurn.data = "dogecoin:DN7WNoyLx6DRoQpuzpcLhV95vLARFdbZ9A?amount=12" // QR generation
QRTurn.gen()
```

# INSTALLATION TO YOUR APP

For Android 

```
String url = "https://dayyoung.github.io/qrturn/scan?returnUrl={YOUR_APP_SCHEME}"
Intent browserIntent = new Intent(Intent.ACTION_VIEW);
browserIntent.setData(Uri.parse(url));
startActivity(browserIntent);

```

For iOS 

```
let goUrl = URL(string: "https://dayyoung.github.io/qrturn/scan?returnUrl={YOUR_APP_SCHEME}")
UIApplication.shared.open(goUrl!, options: [:], completionHandler: nil)
```

# TESTING

 [JSFiddle](https://jsfiddle.net/sx4z0qo9/)

 [Click here for testing : /test.html](/test.html)
 
 [Click here for contacting : dryudryu@gmail.com](mailto:dryudryu@gmail.com)

# LICENSE
[MPL-2.0](https://www.mozilla.org/MPL/2.0/)
