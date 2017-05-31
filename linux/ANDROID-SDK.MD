# Android SDK

#### Show Android Virtual Device Manager ( version 24 or less)
```bash
$ android avd
```


## Commandl line tools
### SDK Manager Install Package

```bash
    sdkmanager --verbose "system-images;android-25;google_apis;x86"
```

### AVD Manager create avd 
```bash
avdmanager create avd --force --name testAVD --abi google_apis/x86 --package system-images;android-25;google_apis;x86

```