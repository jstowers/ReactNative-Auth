## Auth Using Firebase

_Sunday, March 11, 2018_

I tried to install the React Native template but the project would not build.

Received the following error:

```javascript
    https://github.com/facebook/react-native/issues/14423#issuecomment-312334645

    // ERROR:  DOES NOT BUILD
    // Default Configuration
    {
      "name": "auth",
      "version": "0.0.1",
      "private": true,
      "scripts": {
        "start": "node node_modules/react-native/local-cli/cli.js start",
        "test": "jest"
      },
      "dependencies": {
        "react": "^16.3.0-alpha.1",
        "react-native": "0.54.1"
      },
      "devDependencies": {
        "babel-jest": "22.4.1",
        "babel-preset-react-native": "4.0.0",
        "eslint-config-rallycoding": "^3.2.0",
        "jest": "22.4.2",
        "react-test-renderer": "^16.3.0-alpha.1"
      },
      "jest": {
        "preset": "react-native"
      }
    }

    // SOLUTION:
    // Downgraded Configuration from Albums Project
    {
      "name": "albums",
      "version": "0.0.1",
      "private": true,
      "scripts": {
        "start": "node node_modules/react-native/local-cli/cli.js start",
        "test": "jest"
      },
      "dependencies": {
        "axios": "0.18.0",
        "react": "16.2.0",
        "react-native": "0.53.3"
      },
      "devDependencies": {
        "babel-jest": "22.4.1",
        "babel-preset-react-native": "4.0.0",
        "eslint-config-rallycoding": "3.2.0",
        "jest": "22.4.2",
        "react-test-renderer": "16.2.0"
      },
      "jest": {
        "preset": "react-native"
      }
    }
```