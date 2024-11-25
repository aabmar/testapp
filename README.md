Warnings and Deprecations on clean Expo 52 default template
===========================================================

Both Expo 51 and Expo 52 has "props.pointerEvents is deprecated" warnings in the default template.

To recreate:

```
npx create-expo-app testapp
cd testapp
npm run web
```

"hook.js:608 props.pointerEvents is deprecated. Use style.pointerEvents Error Component Stack"

I work on both Mac and Windows, and the warning is the same. I have used Expo 51 and now 52, and the warning is the same.


Pointer Events Warning
======================

When launching the project, the Ponter Events deprecation warning is shown on the console where you run Expo, and in the browser dev console:

```
>npm run web

> testapp@1.0.0 web
> expo start --web

Starting project at C:\Users\mariu\testapp
› Port 8081 is being used by another process
√ Use port 8082 instead? ... yes
Starting Metro Bundler
▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄
█ ▄▄▄▄▄ █▀▀ ███▀  █ ▄▄▄▄▄ █
█ █   █ █▄▀██▀█▄▄██ █   █ █
█ █▄▄▄█ █ ▄ █  █ ██ █▄▄▄█ █
█▄▄▄▄▄▄▄█ █ ▀▄█ ▀ █▄▄▄▄▄▄▄█
█▄▄▀▄▀▀▄▄▀▀█  ▄▀██▀  ▄▀▄▄▀█
█▄█▄ ▄█▄██▀▀  ▀ ▀▄▄▀ ▀▀█▄▄█
██ ▀▀▄▄▄▀▄█▄ █  █▀█ ▄█ ██▀█
█▄▀▀█▀▀▄▀▀▀  █▀██ ▄▄ ▀▀██▄█
█▄▄█▄▄▄▄█ ▀▄█ ▀▄  ▄▄▄ █ ▄ █
█ ▄▄▄▄▄ █▄▀▄▄ █▄  █▄█  ▀ ▄█
█ █   █ █▀▄▀▀▄▄▀▀▄ ▄▄ █▀▄██
█ █▄▄▄█ █▀ ▄▀▄  █  █▄  ▄█▄█
█▄▄▄▄▄▄▄█▄▄▄██▄▄█▄███▄▄█▄▄█

› Metro waiting on exp://192.168.10.55:8082
› Scan the QR code above with Expo Go (Android) or the Camera app (iOS)

› Web is waiting on http://localhost:8082

› Using Expo Go
› Press s │ switch to development build

› Press a │ open Android
› Press w │ open web

› Press j │ open debugger
› Press r │ reload app
› Press m │ toggle menu
› shift+m │ more tools
› Press o │ open project code in your editor

› Press ? │ show all commands

Logs for your project will appear below. Press Ctrl+C to exit.
λ Bundled 26742ms C:\Users\mariu\testapp\node_modules\expo-router\node\render.js (919 modules)
Web C:\Users\mariu\testapp\node_modules\expo-router/entry.js ▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓▓ 100.0% (921/921)λ  WARN  props.pointerEvents is deprecated. Use style.pointerEvents
  console.warn (C:\Users\mariu\testapp\node_modules\@expo\cli\src\start\server\serverLogLikeMetro.ts:91:21)
  warnOnce (C:\Users\mariu\testapp\node_modules\react-native-web\dist\modules\warnOnce\index.js:24:13)
  createDOMProps (C:\Users\mariu\testapp\node_modules\react-native-web\dist\modules\createDOMProps\index.js:805:13)
  createElement (C:\Users\mariu\testapp\node_modules\react-native-web\dist\exports\createElement\index.js:23:32)
  Component (C:\Users\mariu\testapp\node_modules\react-native-web\dist\exports\View\index.js:111:23)
  renderWithHooks (C:\Users\mariu\testapp\node_modules\react-dom\cjs\react-dom-server-legacy.node.development.js:5662:16)
  renderForwardRef (C:\Users\mariu\testapp\node_modules\react-dom\cjs\react-dom-server-legacy.node.development.js:5857:18)
  renderElement (C:\Users\mariu\testapp\node_modules\react-dom\cjs\react-dom-server-legacy.node.development.js:6020:11)
  renderNodeDestructiveImpl (C:\Users\mariu\testapp\node_modules\react-dom\cjs\react-dom-server-legacy.node.development.js:6119:11)
  renderNodeDestructive (C:\Users\mariu\testapp\node_modules\react-dom\cjs\react-dom-server-legacy.node.development.js:6091:14)
Web Bundled 28463ms C:\Users\mariu\testapp\node_modules\expo-router\entry.js (921 modules)
Web Bundled 9082ms C:\Users\mariu\testapp\node_modules\expo-router\entry.js (921 modules)
 LOG  [web] Logs will appear in the browser console

```


Deprecation Warning
===================

During create-expo-app's work, these deprecation warnings will appear on the console:


```

>npx create-expo-app testapp
Creating an Expo project using the default template.

To choose from all available templates pass in the --template arg:
  $ npx create-expo-app --template

To choose from all available examples pass in the --example arg:
  $ npx create-expo-app --example

√ Downloaded and extracted project files.
> npm install
npm WARN deprecated inflight@1.0.6: This module is not supported, and leaks memory. Do not use it. Check out lru-cache if you want a good and tested way to coalesce async requests by a key value, which is much more comprehensive and powerful.
npm WARN deprecated @babel/plugin-proposal-nullish-coalescing-operator@7.18.6: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-nullish-coalescing-operator instead.
npm WARN deprecated @babel/plugin-proposal-class-properties@7.18.6: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-class-properties instead.
npm WARN deprecated rimraf@2.6.3: Rimraf versions prior to v4 are no longer supported
npm WARN deprecated @babel/plugin-proposal-optional-chaining@7.21.0: This proposal has been merged to the ECMAScript standard and thus this plugin is no longer maintained. Please use @babel/plugin-transform-optional-chaining instead.
npm WARN deprecated rimraf@3.0.2: Rimraf versions prior to v4 are no longer supported
npm WARN deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
npm WARN deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
npm WARN deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
npm WARN deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
npm WARN deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
npm WARN deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
npm WARN deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
npm WARN deprecated glob@7.2.3: Glob versions prior to v9 are no longer supported
npm WARN deprecated abab@2.0.6: Use your platform's native atob() and btoa() methods instead
npm WARN deprecated domexception@4.0.0: Use your platform's native DOMException instead
npm WARN deprecated @xmldom/xmldom@0.7.13: this version is no longer supported, please update to at least 0.8.*

added 1179 packages, and audited 1180 packages in 57s

104 packages are looking for funding
  run `npm fund` for details

5 low severity vulnerabilities

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.

✅ Your project is ready!

To run your project, navigate to the directory and run one of the following npm commands.

- cd testapp
- npm run android
- npm run ios # you need to use macOS to build the iOS project - use the Expo app if you need to do iOS development without a Mac
- npm run web

```

