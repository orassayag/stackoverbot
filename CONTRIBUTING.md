# Contributing

Contributions to this project are [released](https://help.github.com/articles/github-terms-of-service/#6-contributions-under-repository-license) to the public under the [project's open source license](LICENSE).

Everyone is welcome to contribute to this project. Contributing doesn't just mean submitting pull requests—there are many different ways for you to get involved, including answering questions, reporting issues, improving documentation, or suggesting new features.

## How to Contribute

### Reporting Issues

If you find a bug or have a feature request:
1. Check if the issue already exists in the [GitHub Issues](https://github.com/orassayag/stackoverbot/issues)
2. If not, create a new issue with:
   - Clear title and description
   - Steps to reproduce (for bugs)
   - Expected vs actual behavior
   - Error codes (if applicable)
   - Your environment details (OS, Node version)

### Submitting Pull Requests

1. Fork the repository
2. Create a new branch for your feature/fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes following the code style guidelines below
4. Test your changes thoroughly
5. Commit with clear, descriptive messages
6. Push to your fork and submit a pull request

### Code Style Guidelines

This project uses:
- **Node.js** with modern JavaScript
- **NPM** for package management
- **Puppeteer** for web automation

Before submitting:
```bash
# Install dependencies
npm install

# Test your changes
npm start
```

### Coding Standards

1. **Clear naming**: Use descriptive names for variables and functions
2. **Error handling**: Implement proper error handling with meaningful messages
3. **Documentation**: Comment complex logic and automation flows
4. **Type safety**: Use proper type checking where applicable
5. **No hardcoded credentials**: Always use environment variables or configuration files
6. **Ethical use**: Ensure automation respects Stack Overflow's terms of service and rate limits

### Adding New Features

When adding new features:
1. Create appropriate configuration options
2. Add service logic for the new functionality
3. Update documentation
4. Test thoroughly on a development account
5. Ensure compliance with Stack Overflow's API and automation policies

### Stack Overflow API Compliance

This project must comply with Stack Overflow's:
- API usage guidelines
- Rate limiting policies
- Terms of service
- Automation best practices

Always:
1. Test on development accounts first
2. Implement proper rate limiting
3. Respect captcha and authentication mechanisms
4. Add delays between operations
5. Monitor for and handle error responses

## Questions or Need Help?

Please feel free to contact me with any question, comment, pull-request, issue, or any other thing you have in mind.

* Or Assayag <orassayag@gmail.com>
* GitHub: https://github.com/orassayag
* StackOverflow: https://stackoverflow.com/users/4442606/or-assayag?tab=profile
* LinkedIn: https://linkedin.com/in/orassayag

Thank you for contributing!
