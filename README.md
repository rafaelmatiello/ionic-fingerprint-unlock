# ionic-fingerprint
Try finger print in ionic, to unlock device.

## Use

1) add a provider FingerprintAIO how module in app.module.ts

import { FingerprintAIO } from '@ionic-native/fingerprint-aio/ngx';

2) How to check unlock
 - check if is fingerprint avaliable
 - show dialog do read a fingerprint

Check code in: src\app\home\home.page.ts

## Commands to install

* ionic start fingerprintApp sidemenu
* ionic cordova plugin add cordova-plugin-fingerprint-aio
* npm install --save @ionic-native/fingerprint-aio
* cordova plugin add cordova-plugin-fingerprint-aio --variable FACEID_USAGE_DESCRIPTION="Login now...."


## Run
* adb devices

* ionic cordova run android -l

## Errors

### Error: net::ERR_CLEARTEXT_NOT_PERMITTED

AndroidManifest.xml

<application ... adicionar android:usesCleartextTraffic="true">
