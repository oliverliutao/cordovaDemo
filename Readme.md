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



## fix issues:
### 1. No Java files found that extend CordovaActivity.
```
cordova platform rm android
cordova platform add android@10.0.0
```

