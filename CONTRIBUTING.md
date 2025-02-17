# Contributing

**Pull requests are welcome!**

If you encounter a problem with OneTimePassword, feel free to [open an issue][issues]. If you know how to fix the bug or implement the desired feature, a pull request is even better.

A great pull request:
- Follows the coding style and conventions of the project.
- Adds tests to cover the added functionality or fixed bug.
- Is accompanied by a clear explanation of its purpose.
- Remains as simple as possible while achieving its intended goal.

Please note that this project is released with a [Contributor Code of Conduct][conduct]. By participating in this project you agree to abide by its terms.

[issues]: https://github.com/mattrubin/OneTimePassword/issues
[conduct]: CONDUCT.md


## Getting Started

1. Check out the latest version of the project:
  ```
  git clone https://github.com/mattrubin/OneTimePassword.git
  ```

2. In the OneTimePassword directory, check out the project's dependencies:
  ```
  cd OneTimePassword
  git submodule update --init --recursive
  ```

3. Open the `OneTimePassword.xcodeproj` file.

4. Build and run the "OneTimePassword" scheme.


## Managing Dependencies

OneTimePassword's source dependencies are [Xcode-managed package dependencies][package dependencies].

Additionally, [Carthage][] is used to manage the project's dependency on shared build configuration files. The dependent project is checked out as a submodule.

To check out the dependencies, simply follow the "Getting Started" instructions above.

To update the dependencies, modify the [Cartfile][] and run:
```
carthage update --no-build --use-submodules
```

[package dependencies]: https://developer.apple.com/documentation/xcode/adding-package-dependencies-to-your-app
[Carthage]: https://github.com/Carthage/Carthage
[Cartfile]: https://github.com/mattrubin/OneTimePassword/blob/develop/Cartfile
