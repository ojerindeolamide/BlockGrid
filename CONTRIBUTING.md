# Contributing to BlockGrid

Thank you for your interest in contributing to BlockGrid! This document provides guidelines and information for contributors.

## 🚀 Getting Started

### Prerequisites

Before contributing, ensure you have:
- [Node.js](https://nodejs.org/) (v16 or higher)
- [Clarinet](https://github.com/hirosystems/clarinet) installed
- [Git](https://git-scm.com/) for version control
- Basic understanding of Clarity smart contracts and Stacks blockchain

### Setting Up Development Environment

1. **Fork the repository**
   ```bash
   # Fork the repo on GitHub, then clone your fork
   git clone https://github.com/YOUR_USERNAME/BlockGrid.git
   cd BlockGrid
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run tests to ensure everything works**
   ```bash
   npm test
   ```

## 🛠 Development Workflow

### Branch Naming Convention

Use descriptive branch names with prefixes:
- `feature/` - New features
- `fix/` - Bug fixes
- `docs/` - Documentation updates
- `refactor/` - Code refactoring
- `test/` - Test improvements

Examples:
- `feature/add-user-authentication`
- `fix/contract-validation-bug`
- `docs/update-api-documentation`

### Making Changes

1. **Create a new branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes**
   - Write clean, readable code
   - Follow existing code style and conventions
   - Add tests for new functionality
   - Update documentation as needed

3. **Test your changes**
   ```bash
   # Run all tests
   npm test
   
   # Run tests with coverage
   npm run test:report
   
   # Run tests in watch mode during development
   npm run test:watch
   ```

4. **Commit your changes**
   ```bash
   git add .
   git commit -m "feat: add new feature description"
   ```

### Commit Message Convention

Follow conventional commit format:
- `feat:` - New features
- `fix:` - Bug fixes
- `docs:` - Documentation changes
- `style:` - Code style changes (formatting, etc.)
- `refactor:` - Code refactoring
- `test:` - Adding or updating tests
- `chore:` - Maintenance tasks

Examples:
- `feat: add grid validation functionality`
- `fix: resolve contract deployment issue`
- `docs: update README with new examples`

## 🧪 Testing Guidelines

### Writing Tests

- Write comprehensive tests for all new functionality
- Use descriptive test names that explain what is being tested
- Test both success and failure scenarios
- Ensure tests are isolated and don't depend on external state

### Test Structure

```typescript
describe("Feature Name", () => {
  it("should do something specific", () => {
    // Arrange
    const input = "test data";
    
    // Act
    const result = functionUnderTest(input);
    
    // Assert
    expect(result).toBe(expectedOutput);
  });
});
```

### Running Tests

```bash
# Run all tests
npm test

# Run tests with coverage and cost reports
npm run test:report

# Watch mode for continuous testing
npm run test:watch
```

## 📝 Code Style Guidelines

### Clarity Smart Contracts

- Use clear, descriptive function and variable names
- Add comprehensive comments for complex logic
- Follow Clarity best practices and conventions
- Use proper error handling with meaningful error codes

### TypeScript/JavaScript

- Use TypeScript for type safety
- Follow existing code formatting
- Use meaningful variable and function names
- Add JSDoc comments for public functions

## 🔍 Code Review Process

1. **Submit a Pull Request**
   - Provide a clear description of changes
   - Reference any related issues
   - Include screenshots for UI changes
   - Ensure all tests pass

2. **Review Criteria**
   - Code quality and readability
   - Test coverage
   - Documentation updates
   - Performance considerations
   - Security implications

3. **Addressing Feedback**
   - Respond to review comments promptly
   - Make requested changes in new commits
   - Update the PR description if scope changes

## 🐛 Reporting Issues

### Bug Reports

When reporting bugs, include:
- Clear description of the issue
- Steps to reproduce
- Expected vs actual behavior
- Environment details (OS, Node.js version, etc.)
- Error messages or logs

### Feature Requests

For feature requests, provide:
- Clear description of the proposed feature
- Use case and motivation
- Possible implementation approach
- Any relevant examples or mockups

## 📚 Resources

- [Stacks Documentation](https://docs.stacks.co/)
- [Clarity Language Reference](https://docs.stacks.co/clarity/)
- [Clarinet Documentation](https://docs.hiro.so/clarinet/)
- [TypeScript Handbook](https://www.typescriptlang.org/docs/)

## 🤝 Community Guidelines

- Be respectful and inclusive
- Help others learn and grow
- Provide constructive feedback
- Follow the project's code of conduct

## 📄 License

By contributing to BlockGrid, you agree that your contributions will be licensed under the MIT License.

## ❓ Questions?

If you have questions about contributing, feel free to:
- Open an issue for discussion
- Reach out to the maintainers
- Check existing documentation and issues

Thank you for contributing to BlockGrid! 🎉
