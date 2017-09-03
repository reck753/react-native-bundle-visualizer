# react-native-bundle-visualizer

See what's inside of your react-native bundle 📦

![bundle-visualizer-animation](./react-native-bundle-visualizer.gif)

Uses the awesome [webpack-visualizer](https://github.com/chrisbateman/webpack-visualizer) and [haul](https://github.com/callstack-io/haul) bundler.

## Purpose

Sometimes, importing a single javascript library can drastically increase your bundle size. This library helps you to identify such a library, so you can keep the bundle size low and loading times fast.

## Usage

Install as a dev dependency:

	yarn add --dev react-native-bundle-visualizer
	or
	npm i --save-dev react-native-bundle-visualizer
	
And run it:

	$ react-native-bundle-visualizer

### Gitignore output files

Additionally, add the haul generated `dist` and `.happypack` folders to your `.gitignore` file:

```
dist/
.happypack/
```

## Disclaimer

The sizes reported are an indication rather than the exact byte size in your bundle. This is because the Haul packager returns different bundles compared to the react-native Metro bundler. Also, due to limitations in webpack's stats, the "actual" (minified) numbers reported here are approximate, but they should be pretty close.

## License

[MIT](./LICENSE.txt)
