# frontend-component-cookie-policy-banner

[![Greenkeeper badge](https://badges.greenkeeper.io/edx/frontend-component-cookie-policy-banner.svg)](https://greenkeeper.io/)
[![npm](https://img.shields.io/npm/v/@edx/frontend-component-cookie-policy-banner.svg)](https://www.npmjs.com/package/@edx/frontend-component-cookie-policy-banner)
[![npm](https://img.shields.io/npm/dt/@edx/frontend-component-cookie-policy-banner.svg)](https://www.npmjs.com/package/@edx/frontend-component-cookie-policy-banner)

## Introduction

edX cookie policy banner React component

## Installation

```bash
npm i --save @edx/frontend-component-cookie-policy-banner
```

## Usage

```jsx
import CookiePolicyBanner from '@edx/frontend-component-cookie-policy-banner';

// Can import sass file this way
// Or as an import in one of your sass files with other third party sass files
import '@edx/frontend-component-cookie-policy-banner/build/frontend-component-cookie-policy-banner.scss';

const SomeWrappingComponent = () => (
  <div>
    <span>Blahblablah</span>
    <CookiePolicyBanner />
  </div>
);
```

### Styling

As noted in a comment in the previous code example, you can import the styles associated with the `CookiePolicyBanner` component directly (if this is supported by your `webpack` config) or by importing the sass file as part of one of your existing sass files (probably where your other third-party sass files are imported).


Requirement: | The `CookiePolicyBanner` sass file assumes the presence of an @edx/brand theme
:---: | :---

```sass
// base.scss
@import 'thirdPartySass';
@import 'anotherThirdPartySass';

// Theme styles
@import '@edx/brand/paragon/fonts';
@import '@edx/brand/paragon/variables';

// Cookie Policy Banner style
@import '@edx/frontend-component-cookie-policy-banner/build/frontend-component-cookie-policy-banner';
```

## Storybook

![storybook](https://imgur.com/mZct2v5.png)

[`Storybook`](https://github.com/storybooks/storybook) is a useful tool for showcasing the expected and potential usage of components.

Executing

As of Nov 2020, Storybook isn't compatible with webpack 5, so before running change your webpack version to 4.44.1.

```bash
npm run start
```

locally builds the Storybook for the `CookiePolicyBanner` component on port `3003`.
