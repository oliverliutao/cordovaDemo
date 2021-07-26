# Android
## add android:

```
cordova platform add android@10.0.0
```

## add plugin:
```
cordova plugin add cordova-plugin-inappbrowser
```


## run
```
cordova run android
```

## build APK in Android studio
### below information required
#### Keystore: Keystore.jks
#### Keystore password 
#### Key Alias name, extract via keytool command
```
keytool -list -v -keystore keystore.jks
```
#### Key password(same as 'keystore password')

## fix issues:
### 1. No Java files found that extend CordovaActivity.
```
cordova platform rm android
cordova platform add android@10.0.0
```

