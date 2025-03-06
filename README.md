# Minecraft Bedrock Versions

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A simple, up-to-date collection of valid Minecraft Bedrock Edition versions in JSON format.

## Overview

This repository provides a comprehensive list of Minecraft Bedrock Edition versions in a JSON format that's easy to consume in applications. The list is maintained to include the latest versions as they are released.

## Usage

### Direct Access

You can directly access the JSON file at:
- [minecraft-bedrock-versions.json](./minecraft-bedrock-versions.json)

### Raw URL

For programmatic access, use the raw GitHub URL:
```javascript
// Example using fetch
fetch('https://raw.githubusercontent.com/yourusername/minecraft-bedrock-versions/main/minecraft-bedrock-versions.json')
  .then(response => response.json())
  .then(data => {
    console.log('Available versions:', data.versions);
    console.log('Latest version:', data.versions[0].value);
  });
```

## Contributing

We welcome contributions to keep the version list up-to-date! Please follow these guidelines when contributing:

### Contribution Guidelines

1. **Version Updates**
   - Only add official Minecraft Bedrock versions
   - Add new versions at the beginning of the versions array
   - Maintain the existing format: `{ "value": "x.xx.xx", "label": "x.xx.xx" }`
   - Verify the version number is correct before submitting

2. **Pull Request Process**
   - Fork the repository
   - Create a new branch for your changes: `git checkout -b feature/add-version-x.xx.xx`
   - Make your changes to the JSON file
   - Test the JSON file for valid syntax
   - Commit with a clear message: `git commit -m "Add version x.xx.xx"`
   - Push to your fork: `git push origin feature/add-version-x.xx.xx`
   - Submit a Pull Request with a clear description of the changes

3. **Code Quality**
   - Ensure the JSON is properly formatted (use a JSON validator)
   - Maintain alphabetical order for imports/requires if adding new code
   - Follow existing code style and conventions

4. **Documentation**
   - Update the "Latest Version" section in README.md if adding a new version
   - Add comments in your PR describing any special considerations

### Code of Conduct

- Be respectful and inclusive in discussions
- Focus on constructive feedback
- Help others learn and grow
- Follow the project's conventions

### Need Help?

If you have questions or need help with your contribution:
1. Open an issue with your question
2. Tag it with the "question" label
3. Provide as much context as possible

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.