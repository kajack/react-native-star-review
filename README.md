<img alt="React Native Star Review" src="https://github.com/WrathChaos/react-native-star-review/blob/master/assets/logo.png" width="1050"/>

Fully customizable Star Review for React Native.

[![npm version](https://img.shields.io/npm/v/react-native-star-review.svg)](https://www.npmjs.com/package/react-native-star-review)
[![npm](https://img.shields.io/npm/dt/react-native-star-review.svg)](https://www.npmjs.com/package/react-native-star-review)
![expo-compatible](https://img.shields.io/badge/Expo-compatible-9cf.svg)
![Platform - Android and iOS](https://img.shields.io/badge/platform-Android%20%7C%20iOS-blue.svg)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![styled with prettier](https://img.shields.io/badge/styled_with-prettier-ff69b4.svg)](https://github.com/prettier/prettier)

<p align="center">
<img alt="React Native Star Review" src="https://github.com/WrathChaos/react-native-star-review/blob/master/assets/Screenshots/example.png" />
</p>

## Installation

Add the dependency:

### Pure React Native:

```ruby
npm i react-native-star-review
```

## Peer Dependencies

###### IMPORTANT! You need install them.

```
"react": ">= 16.x.x",
"react-native": ">= 0.55.x",
"react-number-format": ">= 4.x.x",
"react-native-vector-icons": ">= 6.x.x",
"react-native-dynamic-vector-icons": ">= x.x.x"

// Expo Version
"react-native-dynamic-vector-icons": "WrathChaos/react-native-dynamic-vector-icons#expo"
```

## Basic Usage

```ruby
 <StarReview />
```

## Advanced Usage

You can check the example for the advanced usage

```ruby
<StarReview
  ratings={5}
  stars={10}
  starColor="#8409ff"
  reviews={219301495}
  reviewsText="contributions"
/>
```

### Configuration - Props

| Property          |   Type    | Default | Description                                                 |
| ----------------- | :-------: | :-----: | ----------------------------------------------------------- |
| stars             |  number   |    5    | create stars as many as you want                            |
| reviews           |  number   |    0    | makes the stars fillable as many as you want                |
| reviewsText       |  string   | reviews | change the review's description text                        |
| starSize          |  number   |   16    | change the star icon's size                                 |
| starColor         |  string   | #ffa114 | change the star icon's color                                |
| textColor         |  string   | #757575 | change the text color                                       |
| iconComponent     | component |  Icon   | set your own Icon component instead of dynamic-vector-icons |
| enableStars       |  boolean  |  false  | shows the stars as text                                     |
| enableParentheses |  boolean  |  false  | reviews are shown inside of parentheses                     |

## Expo Compatibility

Star Review is usable with Expo. You just need to add a peer dependency:

```
"react-native-dynamic-vector-icons": "WrathChaos/react-native-dynamic-vector-icons#expo"
```

## Known Issues

### Android

#### Stars are not showing :O

-> You need to add this line of code into app/gradle

```ruby
apply from: "../../node_modules/react-native-vector-icons/fonts.gradle"
```

### ToDos

- [x] LICENSE
- [ ] Write an article about the lib on Medium

## Author

FreakyCoder, kurayogun@gmail.com

## License

React Native Star Review Library is available under the MIT license. See the LICENSE file for more info.
