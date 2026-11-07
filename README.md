# Expo NativeWind Starter

A starter template for building cross-platform apps with Expo, Expo Router, TypeScript, NativeWind, and Tailwind CSS.

## Stack

- Expo SDK 58 and React Native
- Expo Router for file-based navigation
- NativeWind v5 release candidate and Tailwind CSS v4
- TypeScript and ESLint

> **Note:** NativeWind v5 is a release candidate. Its installation guide lists Expo SDK 57 as its tested target; this starter uses SDK 58. Test your app on the platforms you plan to support.

## Getting started

### Requirements

- Node.js 24.3 or newer on the Node 24 release line
- npm
- Expo Go, a development build, or an emulator/simulator for mobile testing

### Installation

Create a repository from this template or clone it, then install dependencies:

```bash
npm ci
```

Start the development server:

```bash
npx expo start
```

Follow the terminal instructions to open the app on your preferred platform. Expo Go must support the Expo SDK version used by this project.

## Project structure

```text
src/
  app/
    _layout.tsx    # Root navigation layout
    index.tsx      # Home screen
  global.css       # Tailwind and NativeWind imports
assets/            # App icons and images
```

Add screens inside `src/app` and use NativeWind utility classes through the `className` prop.

## Commands

```bash
npm run android      # Start for Android
npm run ios          # Start for iOS
npm run web          # Start for web
npm run lint         # Run ESLint
npx tsc --noEmit     # Check TypeScript
```

If styling changes are not picked up, restart Metro with a cleared cache:

```bash
npx expo start --clear
```

## Customize your app

1. Update the app name, slug, and URL scheme in `app.json`.
2. Replace the icons and splash-screen assets.
3. Remove or replace the existing Expo owner and EAS project ID before connecting your own EAS project.
4. Edit the home screen in `src/app/index.tsx` and add your own routes.

## Resources

- [Expo documentation](https://docs.expo.dev/)
- [Expo Router documentation](https://docs.expo.dev/router/introduction/)
- [NativeWind v5 documentation](https://www.nativewind.dev/v5/getting-started/installation)
- [Tailwind CSS documentation](https://tailwindcss.com/docs)

## License

MIT. See [LICENSE](./LICENSE).

