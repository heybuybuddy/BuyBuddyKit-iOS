![alt text](https://github.com/heybuybuddy/BuyBuddyKit-specs/blob/master/images/buybuddy_logo2.png)

# BuyBuddyKit Framework

BuyBuddyKit is a library which contains customizable views and API convenience methods for you to integrate to the BuyBuddy platform and enable your customers to utilize the interface and the capabilities of BuyBuddy shopping experience.

## Requirements

* iOS 9.0+

* Xcode 8.1, 8.2, 8.3, and 9.0

* Swift 3.0, 3.1, 3.2, and 4.0

## Installation

BuyBuddyKit supports multiple methods for installing the library in a project.

### Installation with Carthage

Carthage is a decentralized dependency manager that builds your dependencies and provides you with binary frameworks.

You can install Carthage with Homebrew using the following command:

```ruby
  $ brew update
  $ brew install carthage
```

To integrate BuyBuddyKit into your Xcode project using Carthage, specify it in your Cartfile:

`github "heybuybuddy/BuyBuddyKit-specs" ~> 1.0.0`

Run `carthage update` to build the framework and drag the built `BuyBuddyKit.framework` into your Xcode project.

### Installation with CocoaPods

#### Cocoapods
CocoaPods is a dependency manager for Swift and Objective-C Cocoa projects. It has over 35 thousand libraries and is used in over 2.3 million apps. CocoaPods can help you scale your projects elegantly.

`$ gem install cocoapods`

#### Podfile

To integrate BuyBuddyKit into your Xcode project using CocoaPods, specify it in your Podfile:


```ruby
  use_frameworks!
  
target 'TargetName' do

pod 'BuyBuddyKit', '~> 1.0.1'

end
```
Then, run the following command:

`$ pod install`

### Manually

If you prefer not to use any of the aforementioned dependency managers, you can integrate BuyBuddyKit into your project manually.

#### Embedded Framework

* Open up Terminal, cd into your top-level project directory, and run the following command "if" your project is not initialized as a git repository:

`$ git init`

* Add BuyBuddyKit as a git submodule by running the following command:

`$ git submodule add https://github.com/heybuybuddy/BuyBuddyKit-specs.git`

* Open the new BuyBuddyKit folder, and drag the BuyBuddyKit.framework into the Project Navigator of your application's Xcode project.

> It should appear nested underneath your application's blue project icon. Whether it is above or below all the other Xcode groups does not matter.

* Select the BuyBuddyKit.framework in the Project Navigator and verify the deployment target matches that of your application target.

* Next, select your application project in the Project Navigator (blue project icon) to navigate to the target configuration window and select the application target under the "Targets" heading in the sidebar.

* In the tab bar at the top of that window, open the "General" panel.

* Click on the + button under the "Embedded Binaries" section.

* Select the BuyBuddyKit.framework.

* And that's it!

The BuyBuddyKit.framework is automatically added as a target dependency, linked framework and embedded framework in a copy files build phase which is all you need to build on the simulator and a device.

## Required Libraries

[Alamofire](https://github.com/Alamofire/Alamofire)

[AlamofireImage](https://github.com/Alamofire/AlamofireImage)

[ObjectMapper](https://github.com/Hearst-DD/ObjectMapper)

## Attributions

See  [Attributions](../master/ATTRIBUTIONS)
.

## License

[MIT](../master/LICENSE)
