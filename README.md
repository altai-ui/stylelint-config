# Stylelint config

## Installation

```bash
npm install @qvant/stylelint-config stylelint --save-dev

# or with yarn:
yarn add @qvant/stylelint-config stylelint --dev
```

## Extend stylelint config

We provide a config for both CSS and SCSS. You can choose which one you would like to extend in your configuration:

### CSS

```json
// .stylelintrc

// base rules
{
  "extends": "@qvant/stylelint-config/css/base"
}

// or base rules + prettier reset
{
  "extends": "@qvant/stylelint-config/css/prettier"
}
```

### SCSS

```json
// .stylelintrc

// base rules + scss rules
{
  "extends": "@qvant/stylelint-config/scss/base"
}

// or base rules + scss rules + prettier reset
{
  "extends": "@qvant/stylelint-config/scss/prettier"
}
```

## Add scripts

```json
{
  // ...
  "scripts": {
    // ...
    "lint:style": "stylelint '**/*.{css,scss,vue}'",
    "lint:style:fix": "stylelint --fix '**/*.{css,scss,vue}'"
  }
  // ...
}
```
