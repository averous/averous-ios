# averous

averous iOS SDK enables mobile app performance monitoring and user behavior tracking.

### Integration Instructions

1. You can install the SDK through CocoaPods:

```
target 'MyApp' do
  ...
  pod 'Averous'
  ...
end
```

2. Initialise averous in your **application:didFinishLaunchingWithOptions:** function:

```
import Averous

func application(_ application: UIApplication, didFinishLaunchingWithOptions ....) -> Bool {
    ...
    Averous.shared.start("YOUR_API_KEY")
    return true
}
```


### Important Notes
* SDK uploads last session data whenever the app is about to enter the foreground. 
