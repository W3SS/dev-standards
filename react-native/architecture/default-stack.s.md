# [Standard] React Native stack

## Owner: Florian Rival

## Why

Having a set of common tools/libraries allow us to quickly move from one project to another, be more efficient and get a deep knowledege of each tool, including the advantages **and** drawbacks of these tools.

## React Native

| Library/tool        | What           | Why  | Alternatives
| ------------- |-------------| -----|
| `react-navigation`  | Navigation library for React Native | Recommended solution on [React Native documentation](https://facebook.github.io/react-native/docs/navigation.html), very customizable and with performant good enough for +90% of apps |
| `react-native-vector-icons`  | Customizable Icons for React Native | Most comprehensive library of icons |
| `redux`  | State container | Widely used in the React community, lots of dev tooling  |
| `redux-persist`  | Persistence of the data of the app | Simple to integrate with Redux and flexible |
| `redux-saga`  | Handling of asynchronous processes in the app | Simple to integrate with Redux, testable, make complex business flow easy to read |
| `formik`, `react-native-form-idable`? | Forms handling library |  |
| `date-fns`, `moment` | Date handling library | Widely used libraries.  |
| Lottie (`react-native-lottie`) | Animation library | Good looking, performant animations. Easy to integrate in React Native. |

### Testing

| Library/tool        | What           | Why  |
| ------------- |-------------| -----|
| jest  | Testing framework | Already integrated with React Native by default, allow to do snapshot testing |
| redux-saga-test-plan  | Testing utilities for `redux-saga` | Allow to test redux-saga |
| detox | End to end testing | Alternatives (Calabash) are not reliable enough and slow |

### Tooling

| Library/tool        | What           | Why  |
| ------------- |-------------| -----|
| Prettier  | Automatic formattting of source code | Avoid all discussions/loss of time on styling Integration/plugin for editors  |
| eslint with `eslint-config-universe` | Linter |   |
| Flowtype  | Static typing | Improve developer experience, help to avoid errors when dealing with complex objects |
| AppCenter Code Push  | Deploy mobile app updates without a full release | Speed up the deployment during development, allow for bug fixes and new features releases on the fly |
| Sentry  | Native crashes and JS exceptions reports | Easy integration and good React Native support with `react-native-sentry` |


### Deployment tooling

| Library/tool        | What           | Why  |
| ------------- |-------------| -----|
| fastlane  | Automation of deployment tasks | Most widely used deployment tool for iOS/Android + existing actions for HockeyApp/App Center/App Store/Play Store |
| match  | Automation of certificate/provisioning profile generation | Avoid dealing with certificates, one place storage for all certificates |

### 3rd-party services

| Library/tool        | What           | Why  |
| ------------- |-------------| -----|
| Bitrise  | Automation of applications builds | Ensure reproducible builds, avoid spending time building apps on developer computers |
| Travis CI  | Automation of unit tests |  |
| Firebase Analytics  | Analytics for mobile applications | The recommended solution by Google for applications, with a good quality native module for React Native ([react-native-firebase](https://github.com/invertase/react-native-firebase)) |

