# FLW Theme

## Installation

```bash
npm install @flwconnect/theme
```

## Usage

Import the base CSS once in your application entry:

```javascript
import '@flwconnect/theme/base.css';
```

To use the Tailwind preset, extend your `tailwind.config.js`:

```javascript
import flwPreset from '@flwconnect/theme/tailwind-preset.js';

export default {
  presets: [flwPreset],
  // other Tailwind config options...
};
```

### Overriding tokens

The package exposes design tokens as CSS variables. You can override any token by redefining it after importing `base.css`.

```css
/* app.css */
@import '@flwconnect/theme/base.css';

:root {
  --color-primary: #0f0;
  /* add other overrides here */
}
```

This example updates the primary color token; define your overrides after the import so your values take precedence.
