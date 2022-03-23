# ecdsa_signature_playground_wc

ECDSA signature and verification

For more information see here: http://fluttercrypto.bplaced.net/ecdsa-signature-playground-webcrypto/

```plaintext
https://pub.dev/packages/webcrypto
https://github.com/google/webcrypto.dart
webcrypto: ^0.5.2

https://pub.dev/packages/url_launcher
url_launcher: ^6.0.20

https://pub.dev/packages/path_provider
path_provider: ^2.0.9

load newest version from GitHub:
  webcrypto:
    git:
      url: https://github.com/google/webcrypto.dart.git

in AndroidManifest.xml ergänzen:
    ... </application>
    
    <queries>
        <!-- If your app opens https URLs -->
        <intent>
            <action android:name="android.intent.action.VIEW" />
            <data android:scheme="https" />
        </intent>
    </queries>
```    

EC Private key P-256:
```plaintext
-----BEGIN PRIVATE KEY-----
MIGHAgEAMBMGByqGSM49AgEGCCqGSM49AwEHBG0wawIBAQQgdNB7VQrXPkOyNnuy
8e9vOV6QQW/to+6YFFsXjOtueOGhRANCAASrxApJj+qyMrD0i4UdNNbDJw09LV7D
SYjyPDd3xudK+xns163uN19jUc1S7/rOZrOsvWj/4t3c+EqgRK/EpZLi
-----END PRIVATE KEY-----
```

EC Public key P-256:
```plaintext
-----BEGIN PUBLIC KEY-----
MFkwEwYHKoZIzj0CAQYIKoZIzj0DAQcDQgAEq8QKSY/qsjKw9IuFHTTWwycNPS1e
w0mI8jw3d8bnSvsZ7Net7jdfY1HNUu/6zmazrL1o/+Ld3PhKoESvxKWS4g==
-----END PUBLIC KEY-----
```

Klartext:
```plaintext
Mein wichtiges Geheimnis
```

Sample ECDSA P-256 SHA-1 signature:
```plaintext
{
  "algorithm": "ECDSA curve P-256 SHA-1",
  "plaintext": "TWVpbiB3aWNodGlnZXMgR2VoZWltbmlz",
  "signature": "9PeCBx2sGvT4mehyrHmGwH7B+ldsKh+Y9BgMD484wJL/fjIXYy8PJEWTd4CW3cjt2rWKxJtisvDKSfd4cRb7tg=="
}
```

Sample ECDSA P-256 SHA-256 signature:
```plaintext
{
  "algorithm": "ECDSA curve P-256 SHA-256",
  "plaintext": "TWVpbiB3aWNodGlnZXMgR2VoZWltbmlz",
  "signature": "qeputerB/IiaBMqaGNpyMUmlq8Nn7j7L4SyTo8aIE5ybQYda6OdF7bxOjtZNLhxL6sHtz5CLvRYhpUEwjqM+hw=="
}
```

development environment:
```plaintext
Android Studio Bumblebee | 2021.1.1 Patch 2
Build #AI-211.7628.21.2111.8193401, built on February 17, 2022
Flutter version 2.8.1
Dart version 2.15.1
Runtime version: 11.0.11+0-b60-7772763 aarch64
VM: OpenJDK 64-Bit Server VM by JetBrains s.r.o.
```

tested on:
```plaintext
Android Simulator: 
  Android 11 (SDK 30) Emulator,
  Android 12 SV2 (SDK 31) Emulator, 
  Android 6 (SDK 23) Emulator,
  Android 5 (SDK 21) Emulator.
iOS Simulator:  
  iOS 15 Emulator
  iOS 11.4 Emulator 
```


```plaintext

```


## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
