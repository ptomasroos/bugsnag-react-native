# Steps to create project

1. `react-native init PreCalc`
2. `cd PreCalc`
3. `npm install --save bugsnag-react-native`
4. `react-native link`
5. Update `index.ios.js` to create a Bugsnag client:

```js
import { Client } from 'bugsnag-react-native';

// ...

const bugsnag = new Client('some api key');
```

6. `react-native run-ios` run successfully.
7. Open Xcode, check `Project > Build Phases > Link Binary with Libraries` to see the full list:

![](http://i.imgur.com/wYjvfKx.png)

8. Open Product menu in Xcode and select 'Archive', which completes successfully.