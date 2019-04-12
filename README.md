# SwiftConfettiView
Swift Confetti View ! Who doesn't like confetti?


[![CI Status](https://img.shields.io/travis/ugurethemaydin/SwiftConfettiView.svg?style=flat)](https://travis-ci.org/ugurethemaydin/SwiftConfettiView)
[![Version](https://img.shields.io/cocoapods/v/SwiftConfettiView.svg?style=flat)](https://cocoapods.org/pods/SwiftConfettiView)
[![License](https://img.shields.io/cocoapods/l/SwiftConfettiView.svg?style=flat)](https://cocoapods.org/pods/SwiftConfettiView)
[![Platform](https://img.shields.io/cocoapods/p/SwiftConfettiView.svg?style=flat)](https://cocoapods.org/pods/SwiftConfettiView)


<p align="center">
<img src="https://user-images.githubusercontent.com/3869305/56049372-fc693c00-5d51-11e9-81af-83ecd183b1ec.gif" alt="confetti" width="473.6" height="198">
</p>

It's raining confetti! SwiftConfettiView is the easiest way to add fun, multi-colored confetti to your application and make users feel rewarded. Written in Swift, SwiftConfettiView is a subclass of UIView and is highly customizable. From various types and colors of confetti to different levels of intensity, you can make the confetti as fancy as you want.


To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

## Installation

SwiftConfettiView is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:


```swift
pod 'SwiftConfettiView'
```

And then run:

`$ pod install`

#### Manual Installation
To manually install SwiftConfettiView, simply add `SwiftConfettiView.swift` to your project.

## Usage

Creating a SwiftConfettiView is the same as creating a UIView:

```swift
let confettiView = SwiftConfettiView(frame: self.view.bounds)
```

Don't forget to add the subview!

```swift
self.view.addSubview(confettiView)
```

### Types

Pick one of the preconfigured types of confetti with the `.type` property, or create your own by providing a custom image. This property defaults to the `.Confetti` type.

##### `.Confetti`

![confetti](https://cloud.githubusercontent.com/assets/11940172/11819440/c9db329e-a39a-11e5-9284-b0171bee0f24.gif)

```swift
confettiView.type = .Confetti
```

##### `.Triangle`

![triangle](https://cloud.githubusercontent.com/assets/11940172/11819211/9b8b758a-a399-11e5-8ed3-2eb92f633628.gif)

```swift
confettiView.type = .Triangle
```

##### `.Star`

![star](https://cloud.githubusercontent.com/assets/11940172/11819401/90a2188a-a39a-11e5-8a03-ddca3fb52e72.gif)

```swift
confettiView.type = .Star
```

##### `.Diamond`

![diamond](https://cloud.githubusercontent.com/assets/11940172/11819275/f1c83c08-a399-11e5-8d40-85e9a1879526.gif)

```swift
confettiView.type = .Diamond
```

##### `.Image`

![image](https://cloud.githubusercontent.com/assets/11940172/11819363/5f4f0dba-a39a-11e5-826b-d198113f50dd.gif)

```swift
confettiView.type = .Image(UIImage(named: "smiley"))
```

### Colors

Set the colors of the confetti with the `.colors` property. This property has a default value of multiple colors. 

``` swift
confettiView.colors = [UIColor.redColor(), UIColor.greenColor(), UIColor.blueColor()]
```

### Intensity

The intensity refers to how many particles are generated and how quickly they fall. Set the intensity of the confetti with the `.intensity` property by passing in a value between 0 and 1. The default intensity is 0.5.

``` swift
confettiView.intensity = 0.75
```

### Starting

To start the confetti, use

``` swift
confettiView.startConfetti()
```

### Stopping

To stop the confetti, use

``` swift
confettiView.stopConfetti()
```

### Status

To check if the confetti is active and currently being displayed, use

``` swift
confettiView.isActive()
```

Returns `true` if it is being displayed, and `false` if it is not.


## Author

Uğur Ethem AYDIN, ugur@metromedya.com

## License

SwiftConfettiView is available under the MIT license. See the LICENSE file for more info.

Copyright (c) 2019 Uğur Ethem AYDIN

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

