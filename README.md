# flutter-debug-notes
📒Debug notes of Flutter Development 🐛

## Dart
### 1. `final` vs `const`
Anything that isn't known at compile time should be final over const.

## Signing
### 1. iOS 13.1 Real Device Signing issue
*Error*:
```
Running new app on actual iOS (13.3.1) device crashes on startup: code signature invalid for "path/to/Flutter.framework/Flutter"
```
Ref: https://github.com/flutter/flutter/issues/49504

*Solution*:
It's caused by individual profile. Problem at Apple Dev end. Use Team Profile to sign now.
