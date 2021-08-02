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

## build and sign APK via Cordova command line or Android studio
```
cordova run android --release -- --keystore=path/to/keystore.jks --storePassword=password --alias=aviva_travel --password=password --packageType=apk
```
### below information required
#### Keystore: Keystore.jks
#### Keystore password 
#### Key Alias name, extract via keytool command
```
keytool -list -v -keystore keystore.jks
```
#### Key password(same as 'keystore password')


## Repackage via Promon command line
```
java -jar Shielder.jar app-release.apk --config aviva-android-config.xml --keystore keystore.jks --storepass store-password --keyname aviva_travel --keypass key-password --sigalg SHA256withRSA --digestalg SHA256
```

## fix issues:
### 1. No Java files found that extend CordovaActivity.
```
cordova platform rm android
cordova platform add android@10.0.0
```

