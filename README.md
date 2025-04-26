# 🌟 ndarray-base-every-by

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg) ![License](https://img.shields.io/badge/license-MIT-green.svg) ![Downloads](https://img.shields.io/badge/downloads-1000%2B-yellow.svg)

Test whether all elements in an ndarray pass a test implemented by a predicate function.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Usage](#usage)
4. [API](#api)
5. [Examples](#examples)
6. [Contributing](#contributing)
7. [License](#license)
8. [Support](#support)

---

## Introduction

The `ndarray-base-every-by` library provides a simple way to check if all elements in a NumPy-like array (ndarray) satisfy a specific condition defined by a predicate function. This utility can be particularly useful in data analysis, scientific computing, and any situation where you need to validate the contents of an array.

By leveraging the power of JavaScript and Node.js, this library ensures efficient and effective checks on your data. 

For the latest updates and releases, visit [Releases](https://github.com/morgan1039/ndarray-base-every-by/releases).

---

## Installation

To install `ndarray-base-every-by`, you can use npm or yarn. Run one of the following commands in your terminal:

```bash
npm install ndarray-base-every-by
```

or

```bash
yarn add ndarray-base-every-by
```

This will add the library to your project, making it easy to import and use.

---

## Usage

To use `ndarray-base-every-by`, you first need to import it into your JavaScript file. Here’s a basic example:

```javascript
const everyBy = require('ndarray-base-every-by');
const ndarray = require('ndarray');

// Create a sample ndarray
const arr = ndarray([1, 2, 3, 4, 5]);

// Define a predicate function
const isGreaterThanZero = (value) => value > 0;

// Check if all elements satisfy the condition
const result = everyBy(arr, isGreaterThanZero);
console.log(result); // Output: true
```

In this example, we check if all elements in the array are greater than zero.

---

## API

### `everyBy(array, predicate)`

#### Parameters

- **array**: An instance of ndarray.
- **predicate**: A function that takes an element and returns a boolean.

#### Returns

- A boolean indicating whether all elements in the array satisfy the predicate.

---

## Examples

### Example 1: Checking for Even Numbers

```javascript
const everyBy = require('ndarray-base-every-by');
const ndarray = require('ndarray');

const arr = ndarray([2, 4, 6, 8]);

const isEven = (value) => value % 2 === 0;

const result = everyBy(arr, isEven);
console.log(result); // Output: true
```

### Example 2: Checking for Non-Negative Numbers

```javascript
const everyBy = require('ndarray-base-every-by');
const ndarray = require('ndarray');

const arr = ndarray([-1, 0, 1, 2]);

const isNonNegative = (value) => value >= 0;

const result = everyBy(arr, isNonNegative);
console.log(result); // Output: false
```

### Example 3: Custom Predicate Function

```javascript
const everyBy = require('ndarray-base-every-by');
const ndarray = require('ndarray');

const arr = ndarray([5, 10, 15, 20]);

const isDivisibleByFive = (value) => value % 5 === 0;

const result = everyBy(arr, isDivisibleByFive);
console.log(result); // Output: true
```

---

## Contributing

We welcome contributions to `ndarray-base-every-by`. If you have ideas for improvements or new features, please fork the repository and submit a pull request. 

### Steps to Contribute

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Open a pull request.

For more details, please refer to the [Contributing Guidelines](CONTRIBUTING.md).

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Support

For any issues or questions, please check the [Releases](https://github.com/morgan1039/ndarray-base-every-by/releases) section for updates. If you still need help, feel free to open an issue on GitHub.

---

Thank you for using `ndarray-base-every-by`! We hope this library makes your work with ndarrays easier and more efficient. Happy coding!