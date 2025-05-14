# Sqids Apex: Generate Short Unique IDs from Numbers 🚀

![Version](https://img.shields.io/badge/version-1.0.0-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)

Welcome to the **Sqids Apex** repository! This project is the official Salesforce Apex port of Sqids, a powerful tool designed to generate short unique IDs from numbers. Whether you need to create user-friendly URLs or simply want to manage IDs efficiently, Sqids Apex has you covered.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Releases](#releases)

## Introduction

In today's digital world, managing IDs effectively is crucial. Long numerical IDs can be cumbersome and unappealing. Sqids Apex allows you to convert these long numbers into short, unique IDs, making them easier to handle and share. This repository brings the functionality of Sqids to the Salesforce Apex environment, ensuring seamless integration with your Salesforce applications.

## Features

- **Short Unique IDs**: Generate compact IDs from numbers.
- **Salesforce Integration**: Designed specifically for Salesforce Apex.
- **Easy to Use**: Simple methods for generating IDs.
- **Lightweight**: Minimal overhead for maximum performance.
- **Open Source**: Free to use and modify.

## Installation

To get started with Sqids Apex, clone the repository to your local machine:

```bash
git clone https://github.com/Vyper537/sqids-apex.git
```

Next, navigate to the project directory:

```bash
cd sqids-apex
```

You can now deploy the code to your Salesforce org. Make sure to follow the Salesforce deployment process to ensure everything works smoothly.

## Usage

Using Sqids Apex is straightforward. After installing, you can generate short unique IDs with just a few lines of code. Here’s a simple example:

```apex
Integer number = 123456789;
String shortId = Sqids.generateShortId(number);
System.debug(shortId);
```

This will output a short unique ID corresponding to the input number.

## Examples

Here are some practical examples to illustrate how to use Sqids Apex effectively:

### Example 1: Generating Short IDs

```apex
for (Integer i = 1; i <= 10; i++) {
    String shortId = Sqids.generateShortId(i);
    System.debug('Short ID for ' + i + ': ' + shortId);
}
```

### Example 2: Using Short IDs in URLs

You can use the generated short IDs in URLs to create user-friendly links. For instance:

```apex
String baseUrl = 'https://example.com/item/';
for (Integer i = 1; i <= 10; i++) {
    String shortId = Sqids.generateShortId(i);
    String url = baseUrl + shortId;
    System.debug('URL for item ' + i + ': ' + url);
}
```

## Contributing

We welcome contributions! If you want to improve Sqids Apex, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Open a pull request.

Please ensure your code follows the project's coding standards and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or feedback, please reach out via the GitHub Issues section or contact me directly.

## Releases

You can find the latest releases of Sqids Apex [here](https://github.com/Vyper537/sqids-apex/releases). Make sure to download the latest version and follow the instructions to get started.

To stay updated, check the **Releases** section regularly for new features and fixes.

## Conclusion

Thank you for exploring Sqids Apex! We hope this tool enhances your Salesforce applications by simplifying ID management. Happy coding!