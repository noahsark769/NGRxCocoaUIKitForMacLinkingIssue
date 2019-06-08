This repo demonstrates a linking issue with RxCocoa when compiling with a UIKitForMac target on macOS Catalina Beta.

To reproduce the issue:

```
cd NGRxCocoaUIKitForMacLinkingIssue
bundle install --path vendor/bundle
bundle exec pod install
open NGRxCocoaUIKitForMacLinkingIssue.xcworkspace/
```

Then check the "macOS" box in build settings, and build to "My Mac" to observe that the build fails.