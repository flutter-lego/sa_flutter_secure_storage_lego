[![lego project](https://img.shields.io/badge/powered%20by-lego-blue?logo=github)](https://github.com/melodysdreamj/lego)
[![pub package](https://img.shields.io/pub/v/sa_flutter_secure_storage_lego.svg)](https://pub.dartlang.org/packages/sa_flutter_secure_storage_lego)

# sa_flutter_secure_storage_lego
apply [flutter_secure_storage](https://pub.dev/packages/flutter_secure_storage) under 
[simple_architecture_framework](https://github.com/melodysdreamj/simple_architecture_lego).

##  Installation
1. open terminal in the lego project root directory, enter the following command for install cli.
   and create a new lego project if you don't have one.
```bash
flutter pub global activate lego_cli
lego create
```
2. in terminal, enter the following command for add lego to project.
```bash
lego add sa_flutter_secure_storage_lego
```

## Usage
```dart
Check check = await CheckFlutterSecureStorage.get();
print(check.toMap());

check.s000 = "hello";

await CheckFlutterSecureStorage.upsert(check);

Check check2 = await CheckFlutterSecureStorage.get();
print(check2.toMap());
```
