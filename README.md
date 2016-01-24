# fuse-touchid

![Screenshot](https://raw.githubusercontent.com/bolav/fuse-touchid/master/touch.png)

```
<iOSFingerPrint ux:Global="FingerPrint" />
<JavaScript>
	var fp = require('FingerPrint');
	function auth () {
		console.log("auth");
		fp.auth("We need your fingerprint.", function (success, reason) { if (success) { console.log("We are okay"); } console.log("s: " + success + "("+ reason +")"); });
	}
	module.exports = {
		auth: auth
	};
</JavaScript>
```
