# Goal: To have a working react-native app framework that can be built for windows, macos, ios, and android
> Requirements: secure storage, offline database (sqlite)

## stack
- react-native
- react-native-windows
- react-native-macos
- react-native-keychain
- op-sqlite
- tamagui

## @op-engineering/op-sqlite
> sqlite database plugin

- To support macos the podspec needs to have it's minimum version bumped to >= 10.15
- TODO: Submit PR to enable for macos
- TODO: Submit PR to enable for windows

## react-native-flipper-databases
> Flipper plugin for viewing sqlite databases

- This plugin's repo has gone missing but the package is still available on npm
- TODO: Port this plugin to specifically support op-sqlite

## react-native-flipper-op-sqlite
> Flipper plugin for viewing op-sqlite databases

- TODO: New plugin for op-sqlite databases, could potentially be contributed to the mainline repo
- `node_modules/react-native-flipper-databases/src/databasesFlipperPlugin.ts` illustrators how to provide the interface to interoperate with the flipper databases plugin

## react-native-keychain
> https://github.com/oblador/react-native-keychain

- TODO: Add support for windows