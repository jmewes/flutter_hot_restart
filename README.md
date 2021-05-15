# Hot Restart Problem Report

## Steps to reproduce

1. Start app

```
flutter run --verbose -d chrome lib/main.dart
```

2. Edit text in `lib/util/form_stepper/src/form_stepper.dart:6`

```
sed -i 's/continue/discontinue/g' lib/util/form_stepper/src/form_stepper.dart
```

3. Go back to the terminal and press "r"

## References

- https://github.com/flutter/flutter/issues/67194

