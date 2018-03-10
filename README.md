# fawdel

## Set up development environment
* Install brew
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
* Install git
```
brew install --global git
```

* Install node
```
brew install --global node 7.10.1
```
note: react native doesn't work with npm 5 as of now, so don't install the latest node which comes with npm 5. https://github.com/facebook/react-native/issues/14767

* Install yarn
```
brew install --global yarn --without-node
```

* Install awsmobile-cli
```
npm install --global awsmobile-cli
```

* Connect awsmobile with AWS credentials (get credentials from wei)
```
awsmobile-configure
```

* Checkout the source code
```
git clone https://github.com/Fawdel/fawdel.git
```
* Connect to the project in mobile hub
```
awsmobile init 06f188de-23e7-11e8-8184-b1af4e143a3a
```

* Run the app in a simulator
```
npm install & npm run ios
```

# Publish
```
awsmobile publish
```
