# Changelog

## [3.0.0](https://github.com/wadevarine-cpu/auto-read-otp/compare/v2.0.0...v3.0.0) (2026-10-30)


### ⚠ BREAKING CHANGES

* **timer:** rememberCountdownTimerState takes endTimeMillis instead of endDate, and gains an overload taking a Duration. CountdownTimerSize is now CountdownTimerDimensions without textSize, the size parameter is now dimensions, backgroundAlpha is removed, and CountdownTimerState exposes remaining as a Duration instead of getRemainingTimes().
* **input:** the cell slot takes an OtpCellState instead of four parameters, and the built-in cells take state instead of char, focused and isError. textFieldState is renamed to state, inputTransformation is now an extra filter on top of the built-in one, style types are plain classes instead of data classes, and OtpInputFieldState is removed.
* **sms:** SmsUserConsent is replaced by SmsUserConsentEffect. onOTPReceived is now onCodeReceived, smsCodeLength is now codeLength, and onError receives a SmsConsentError instead of a localized string.
* packages moved from com.burkido.autoreadotp and com.burkido.otpinputkit.* to com.burkido.otp.sms, com.burkido.otp.input and com.burkido.otp.timer. The countdown timer is now in the otp-timer artifact.

### Features

* add build-logic convention plugins for library and compose ([03fbd78](https://github.com/wadevarine-cpu/auto-read-otp/commit/03fbd78640ecf56ef749b9c0800797c6ef43b3a5))
* add commit-lint action to enforce conventional commit messages ([7523266](https://github.com/wadevarine-cpu/auto-read-otp/commit/75232669ef8a59b0af08d82cde36ced538844991))
* add OTP styling system with tokens and configurations ([6e20063](https://github.com/wadevarine-cpu/auto-read-otp/commit/6e200639d0cb5473c149051338deefb063a648b5))
* add otp-input-kit and otp-bom modules ([cd578f3](https://github.com/wadevarine-cpu/auto-read-otp/commit/cd578f3fc5d7c2030c2867d9e6fefcf826055652))
* add verification code sample implementation ([990e7cf](https://github.com/wadevarine-cpu/auto-read-otp/commit/990e7cf76e30730953e94276b81b930bfd29257c))
* **app:** add CountdownTimerSamples composable ([14c8316](https://github.com/wadevarine-cpu/auto-read-otp/commit/14c831655c2b08498dd2d908109452144efd0fd6))
* **app:** integrate CountdownTimer into sample screens ([54f5ef9](https://github.com/wadevarine-cpu/auto-read-otp/commit/54f5ef982f754c7d636a71d5350677378f4f7f7f))
* enhance OTP input kit core components ([948c8d8](https://github.com/wadevarine-cpu/auto-read-otp/commit/948c8d8ee4aee86190846030774a4e848098346f))
* **otp-input-kit:** add CountdownTimer composable with state, colors, shape, and size support ([ead2739](https://github.com/wadevarine-cpu/auto-read-otp/commit/ead273996b4f5b1f498172da50995aa59c4e97f1))
* **sample:** add home screen with hero demo ([31bff28](https://github.com/wadevarine-cpu/auto-read-otp/commit/31bff286394434b535e925d13e6e9b2b8a633fcd))
* **sample:** add new theme, shared UI components and icons ([5697be3](https://github.com/wadevarine-cpu/auto-read-otp/commit/5697be358b5b3b80f07611c8d8f9dbcc1866f310))
* **sample:** add OTP design gallery ([38da5f6](https://github.com/wadevarine-cpu/auto-read-otp/commit/38da5f6a56ac645ba4a4ff3dab548f45bd9dce52))
* **sample:** add playground with live configuration ([9514f51](https://github.com/wadevarine-cpu/auto-read-otp/commit/9514f512776326335b64849cae90b7d9cca8a067))
* **sample:** add sign-in flow demo ([99b2f14](https://github.com/wadevarine-cpu/auto-read-otp/commit/99b2f148be88cff108958fad50e7308e61ed5ece))
* **sample:** add SMS lab screen ([24d2bd5](https://github.com/wadevarine-cpu/auto-read-otp/commit/24d2bd5fb090776a6ca004752e59f8e854d91cc1))
* **sample:** redesign sample app ([52439f4](https://github.com/wadevarine-cpu/auto-read-otp/commit/52439f4784e8aecd306a327bd4ff666a66e7f437))
* update OTP cell components and visual styling ([aacd663](https://github.com/wadevarine-cpu/auto-read-otp/commit/aacd66301bbac69e5525ce8a6f5ba51d9c8a28e4))
* update verification screens with enhanced OTP kit ([dbfe8e5](https://github.com/wadevarine-cpu/auto-read-otp/commit/dbfe8e51410a87bfec2d71878be0bf2fb0183e10))


### Bug Fixes

* Correct tag-on-push.yml ([e1ead53](https://github.com/wadevarine-cpu/auto-read-otp/commit/e1ead53d579446c0e7047db572dbf79a13639b11))
* Correct tag-on-push.yml ([c2f738e](https://github.com/wadevarine-cpu/auto-read-otp/commit/c2f738e67225e703f59fbd25ba3cefb3bc508e94))
* Correct tag-on-push.yml ([74b83ac](https://github.com/wadevarine-cpu/auto-read-otp/commit/74b83ac74c23bbb271ac8e5c4be79cb4b3f16e25))
* Correct tag-on-push.yml ([4500f89](https://github.com/wadevarine-cpu/auto-read-otp/commit/4500f8985898faf91cdb823b2a90168975f009d0))
* Correct tag-on-push.yml ([13f5166](https://github.com/wadevarine-cpu/auto-read-otp/commit/13f5166701a2a5637c3205efbe9148483070c598))
* Correct tag-on-push.yml ([5a44d84](https://github.com/wadevarine-cpu/auto-read-otp/commit/5a44d846e80adcac9ece322e8aae2d1cd59592e6))
* Correct tag-on-push.yml ([159dae9](https://github.com/wadevarine-cpu/auto-read-otp/commit/159dae9949cf2d722b27f00f3bb875bab0156924))
* Correct tag-on-push.yml ([6c3228b](https://github.com/wadevarine-cpu/auto-read-otp/commit/6c3228b3387b6d23b034e93db5e5b1c2a164ea8a))
* Correct tag-on-push.yml ([d5d7cb2](https://github.com/wadevarine-cpu/auto-read-otp/commit/d5d7cb2d31ceae2d128e04aebd9d693c5ea086d8))
* Correct tag-on-push.yml ([3546038](https://github.com/wadevarine-cpu/auto-read-otp/commit/3546038c27651f4375db28f1317bc44750205f1d))
* Correct tag-on-push.yml ([bd16f02](https://github.com/wadevarine-cpu/auto-read-otp/commit/bd16f02aa753cd69d7d6bdc2e28ecf8448921ebd))
* Correct yml files ([a0b2b20](https://github.com/wadevarine-cpu/auto-read-otp/commit/a0b2b2027e1b8a64f0c7465232fd3e21a1cd4c23))
* Correct yml files ([bfe179e](https://github.com/wadevarine-cpu/auto-read-otp/commit/bfe179eb6f8c8841299c865823879bf00ad9a8e8))
* Correct yml files ([1ea44c4](https://github.com/wadevarine-cpu/auto-read-otp/commit/1ea44c4442c208578e3d738911653b154dea8ba5))
* Correct yml files ([4442f47](https://github.com/wadevarine-cpu/auto-read-otp/commit/4442f47d3059d4880504908f9edec0f7ae31f000))
* Correct yml files ([cface9c](https://github.com/wadevarine-cpu/auto-read-otp/commit/cface9c3117b467dc4b42a3dcfaee2c19cde067b))
* Correct yml files ([c4340f6](https://github.com/wadevarine-cpu/auto-read-otp/commit/c4340f6864d483c97e8f7fd735b7070d74c69348))
* Correct yml files ([5e07da4](https://github.com/wadevarine-cpu/auto-read-otp/commit/5e07da4ab83e5e957668d96b14e9ce335796d376))
* Correct yml files ([664c63a](https://github.com/wadevarine-cpu/auto-read-otp/commit/664c63a89829d678d7215b05ee2cac5b8e3f9c65))
* Correct yml files ([a23fadc](https://github.com/wadevarine-cpu/auto-read-otp/commit/a23fadc554a0cace37e9134c66238560835feda4))
* Correct yml files ([5c012e0](https://github.com/wadevarine-cpu/auto-read-otp/commit/5c012e03f35fa752d8e20ce15237fb3e0bd26cf3))
* Correct yml files ([3c1d8bc](https://github.com/wadevarine-cpu/auto-read-otp/commit/3c1d8bcd65533ca6e705573a42125d3cc4c04653))
* Correct yml files ([fce575d](https://github.com/wadevarine-cpu/auto-read-otp/commit/fce575d8c7bfdef6dcfbc6a1fbd887cf7f27d005))
* Correct yml files ([ee5b982](https://github.com/wadevarine-cpu/auto-read-otp/commit/ee5b98269cd4d73e01cc17e298d3783304ae6d64))
* Correct yml files ([47dd2f4](https://github.com/wadevarine-cpu/auto-read-otp/commit/47dd2f47ca31e71d30df9f785f50153b6bef86d8))
* Correct yml files ([5f54d2b](https://github.com/wadevarine-cpu/auto-read-otp/commit/5f54d2b79ec2f740c8d811cc5a5fcfa8fd81eebd))
* Correct yml files ([2655b26](https://github.com/wadevarine-cpu/auto-read-otp/commit/2655b269d0ca4045c595617ddd09f32bbdb59a07))
* Correct yml files ([bc52a62](https://github.com/wadevarine-cpu/auto-read-otp/commit/bc52a62207a071183d97d4354d5b22bff83e58c0))
* Correct yml files ([9476e74](https://github.com/wadevarine-cpu/auto-read-otp/commit/9476e74a9a7e0da96ae63ca3c335513f65b08a8a))
* Correct yml files ([aa9ea21](https://github.com/wadevarine-cpu/auto-read-otp/commit/aa9ea2104cc86964a57d48b70066d3de18470d2c))
* Correct yml files ([4be4469](https://github.com/wadevarine-cpu/auto-read-otp/commit/4be4469fd7b30c182635068026d78fe79a1bc324))
* Correct yml files ([d2fe866](https://github.com/wadevarine-cpu/auto-read-otp/commit/d2fe866e94224f5f8d206e1b4e3d9e6a343d638d))
* Correct yml files ([f393c46](https://github.com/wadevarine-cpu/auto-read-otp/commit/f393c46d89620abff85321e418f1c73d17c1155b))
* Correct yml files ([9b92da3](https://github.com/wadevarine-cpu/auto-read-otp/commit/9b92da38f1e1a4ce9606925edf7744ca5989d687))
* Correct yml files ([3d1dc65](https://github.com/wadevarine-cpu/auto-read-otp/commit/3d1dc6552d13b566dbe519a704cd5e75bf88440b))
* Correct yml files ([1340079](https://github.com/wadevarine-cpu/auto-read-otp/commit/1340079aaf1c6da01f4dc2b461d249f33fdef795))
* Correct yml files ([e0ef7e9](https://github.com/wadevarine-cpu/auto-read-otp/commit/e0ef7e9b3210e522e01c7e7cc7a751ebb717a43e))
* Correct yml files ([00a176e](https://github.com/wadevarine-cpu/auto-read-otp/commit/00a176e05ec77fa5680c208bc5ae7bbdf05ce93c))
* **input:** decorator based field, autofill, accessibility, API cleanup ([ac93172](https://github.com/wadevarine-cpu/auto-read-otp/commit/ac931728f82e325dc822b4a68617540a07b890ce))
* **sms:** secure consent flow, correct code parsing, typed errors ([88f3be8](https://github.com/wadevarine-cpu/auto-read-otp/commit/88f3be82a5fcdfe3e32b00db2d03857908ef236a))
* **timer:** coroutine countdown, single text size, screen reader text ([466e9e4](https://github.com/wadevarine-cpu/auto-read-otp/commit/466e9e4b52317c37aaa0784de306b8b85b66374c))
* use BoxScope receiver for hiddenTextField to enable matchParentSize ([5df9e0c](https://github.com/wadevarine-cpu/auto-read-otp/commit/5df9e0ca35f27a92204e751e39cdaaf2b8b48b0c))


### Code Refactoring

* rename modules and packages, split otp-timer ([225b9db](https://github.com/wadevarine-cpu/auto-read-otp/commit/225b9db7a434743eb61be651dfdbf89d5e49d706))

## [2.0.0](https://github.com/burkido/auto-read-otp/compare/v1.2.0...v2.0.0) (2026-10-28)


### ⚠ BREAKING CHANGES

* **timer:** rememberCountdownTimerState takes endTimeMillis instead of endDate, and gains an overload taking a Duration. CountdownTimerSize is now CountdownTimerDimensions without textSize, the size parameter is now dimensions, backgroundAlpha is removed, and CountdownTimerState exposes remaining as a Duration instead of getRemainingTimes().
* **input:** the cell slot takes an OtpCellState instead of four parameters, and the built-in cells take state instead of char, focused and isError. textFieldState is renamed to state, inputTransformation is now an extra filter on top of the built-in one, style types are plain classes instead of data classes, and OtpInputFieldState is removed.
* **sms:** SmsUserConsent is replaced by SmsUserConsentEffect. onOTPReceived is now onCodeReceived, smsCodeLength is now codeLength, and onError receives a SmsConsentError instead of a localized string.
* packages moved from com.burkido.autoreadotp and com.burkido.otpinputkit.* to com.burkido.otp.sms, com.burkido.otp.input and com.burkido.otp.timer. The countdown timer is now in the otp-timer artifact.

### Features

* **sample:** add home screen with hero demo ([31bff28](https://github.com/burkido/auto-read-otp/commit/31bff286394434b535e925d13e6e9b2b8a633fcd))
* **sample:** add new theme, shared UI components and icons ([5697be3](https://github.com/burkido/auto-read-otp/commit/5697be358b5b3b80f07611c8d8f9dbcc1866f310))
* **sample:** add OTP design gallery ([38da5f6](https://github.com/burkido/auto-read-otp/commit/38da5f6a56ac645ba4a4ff3dab548f45bd9dce52))
* **sample:** add playground with live configuration ([9514f51](https://github.com/burkido/auto-read-otp/commit/9514f512776326335b64849cae90b7d9cca8a067))
* **sample:** add sign-in flow demo ([99b2f14](https://github.com/burkido/auto-read-otp/commit/99b2f148be88cff108958fad50e7308e61ed5ece))
* **sample:** add SMS lab screen ([24d2bd5](https://github.com/burkido/auto-read-otp/commit/24d2bd5fb090776a6ca004752e59f8e854d91cc1))
* **sample:** redesign sample app ([52439f4](https://github.com/burkido/auto-read-otp/commit/52439f4784e8aecd306a327bd4ff666a66e7f437))


### Bug Fixes

* **input:** decorator based field, autofill, accessibility, API cleanup ([ac93172](https://github.com/burkido/auto-read-otp/commit/ac931728f82e325dc822b4a68617540a07b890ce))
* **sms:** secure consent flow, correct code parsing, typed errors ([88f3be8](https://github.com/burkido/auto-read-otp/commit/88f3be82a5fcdfe3e32b00db2d03857908ef236a))
* **timer:** coroutine countdown, single text size, screen reader text ([466e9e4](https://github.com/burkido/auto-read-otp/commit/466e9e4b52317c37aaa0784de306b8b85b66374c))


### Code Refactoring

* rename modules and packages, split otp-timer ([225b9db](https://github.com/burkido/auto-read-otp/commit/225b9db7a434743eb61be651dfdbf89d5e49d706))

## Changelog

All notable changes are listed here. Entries are generated by release-please from Conventional Commit messages.
