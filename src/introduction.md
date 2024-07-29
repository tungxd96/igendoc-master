## Introduction

Welcome to the Lorem Ipsum API documentation. This API allows you to generate placeholder text for your applications.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

## Installation

To use the Lorem Ipsum API in your project, you need to install the necessary dependencies.

### Using npm

```bash
npm install lorem-ipsum-api
```

### Using yarn

```bash
yarn add lorem-ipsum-api
```

## Usage

Here are some examples of how to use the Lorem Ipsum API in your application.

### Basic Example

```javascript
import { generateLoremIpsum } from "lorem-ipsum-api";

const loremText = generateLoremIpsum();
console.log(loremText);
```

### Custom Options

You can customize the generated text by providing options.

```javascript
import { generateLoremIpsum } from "lorem-ipsum-api";

const options = {
  count: 5, // Number of words, sentences, or paragraphs
  units: "paragraphs", // 'words', 'sentences', or 'paragraphs'
};

const loremText = generateLoremIpsum(options);
console.log(loremText);
```

## API Reference

### generateLoremIpsum(options)

Generates Lorem Ipsum text based on the provided options.

#### Parameters

- `options` (optional) - An object containing the following properties:
  - `count` (number) - The number of words, sentences, or paragraphs to generate. Default is `1`.
  - `units` (string) - The unit of text to generate: `'words'`, `'sentences'`, or `'paragraphs'`. Default is `'words'`.

#### Returns

- A string containing the generated Lorem Ipsum text.

#### Example

```javascript
import { generateLoremIpsum } from "lorem-ipsum-api";

const options = {
  count: 3,
  units: "sentences",
};

const loremText = generateLoremIpsum(options);
console.log(loremText);
```
