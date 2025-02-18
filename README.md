# React Native plugin for Reader SDK

[![Build Status](https://travis-ci.com/square/react-native-square-reader-sdk.svg?branch=master)](https://travis-ci.com/square/react-native-square-reader-sdk)
[![npm version](https://badge.fury.io/js/react-native-square-reader-sdk.svg)](https://badge.fury.io/js/react-native-square-reader-sdk)
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FAremixdj%2Freact-native-square-reader-sdk.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FAremixdj%2Freact-native-square-reader-sdk?ref=badge_shield)

This repo contains a React Native plugin for Square [Reader SDK]. Reader SDK for
React Native supports the following native Reader SDK versions:

  * iOS: 1.7.2 and above
  * Android: 1.7.5 and above

>This plugin loads latest version of native Reader SDK by default according to [update policy for Reader SDK].

## In this repo

In addition to the standard React Native directories, this repo includes:

* `docs` - Documentation for the React Native plugin, including a
  [getting started guide], [technical reference], and [troubleshooting guide].
* [`reader-sdk-react-native-quickstart`] - A React Native sample app with
  walkthrough.


## Build requirements

### Android

* minSdkVersion is API 24 or higher.
* Android SDK platform: API 30.
* Android SDK build tools: 28.0.3
* Android Gradle Plugin: 3.0.0 or greater.
* Support library: 28.0.0
* Google Play Services: 16.0.1
* Google APIs Intel x86 Atom_64 System Image

### iOS

* Xcode version: 10.2 or greater.
* iOS Base SDK: 11.1 or greater.
* Deployment target: iOS 11.0 or greater.


## Reader SDK requirements and limitations

* Reader SDK is **only** available for accounts based in the **United States**.
  Authorization requests for accounts based outside the United States return an
  error.
* Reader SDK may not be used for unattended terminals. Using Reader SDK to
  implement payment solutions in unattended terminals or kiosks (for example,
  vending machines) is strictly prohibited.
* Reader SDK requires an authorization token from the [Mobile Authorization API]
  to connect Square Readers and accept payments.
* Reader SDK only supports on-screen tipping. Digital receipts and tips can be
  configured in Reader SDK. Tipping on printed receipts is not supported at this
  time.
* Reader SDK cannot issue refunds. Refunds can be issued programmatically using
  the Refunds API or manually in the [Square Dashboard].
* Reader SDK is not supported in the Square sandbox. See [Testing Mobile Apps]
  for testing recommendations.
* Your version of Reader SDK must adhere to the Square SDK update policy. To
  limit risk to developers and their users, Square enforces an
  [update policy for Reader SDK] that requires developers to keep their version
  of Reader SDK current.


## License

```
Copyright 2019 Square Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```


[//]: # "Link anchor definitions"
[Mobile Authorization API]: https://developer.squareup.com/docs/mobile-authz/build-with-mobile-authz
[Reader SDK]: https://developer.squareup.com/docs/reader-sdk/what-it-does
[Square Dashboard]: https://squareup.com/dashboard/
[update policy for Reader SDK]: https://developer.squareup.com/docs/reader-sdk/what-it-does#readersdkupdatepolicy
[Testing Mobile Apps]: https://developer.squareup.com/docs/testing/mobile
[getting started guide]: https://github.com/square/react-native-square-reader-sdk/tree/master/docs/get-started.md
[technical reference]: https://github.com/square/react-native-square-reader-sdk/tree/master/docs/reference.md
[troubleshooting guide]: https://github.com/square/react-native-square-reader-sdk/tree/master/docs/troubleshooting.md
[`reader-sdk-react-native-quickstart`]: https://github.com/square/react-native-square-reader-sdk/tree/master/reader-sdk-react-native-quickstart


[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FAremixdj%2Freact-native-square-reader-sdk.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FAremixdj%2Freact-native-square-reader-sdk?ref=badge_large)