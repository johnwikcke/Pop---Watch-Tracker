# 🤝 Contributing to Pop Watch Tracker

Thank you for your interest in contributing to Pop Watch Tracker! This document provides guidelines and information for contributors.

## 🌟 Ways to Contribute

- 🐛 **Report bugs** - Help us identify and fix issues
- 💡 **Suggest features** - Share ideas for new functionality
- 📝 **Improve documentation** - Help make our docs clearer
- 🔧 **Submit code** - Fix bugs or implement new features
- 🎨 **Design improvements** - Enhance UI/UX
- 📱 **Android development** - Improve the native Android app
- 🧪 **Testing** - Help test on different devices and browsers

## 🚀 Getting Started

### Prerequisites
- Git
- Text editor or IDE
- Web browser for testing
- Android Studio (for Android development)

### Setup Development Environment

1. **Fork the repository**
   ```bash
   # Click "Fork" on GitHub, then clone your fork
   git clone https://github.com/yourusername/pop-watch-tracker.git
   cd pop-watch-tracker
   ```

2. **Create a branch**
   ```bash
   git checkout -b feature/your-feature-name
   # or
   git checkout -b fix/bug-description
   ```

3. **Set up for web development**
   ```bash
   # Simple HTTP server for testing
   python -m http.server 8000
   # or
   npx serve .
   ```

4. **Set up for Android development**
   ```bash
   # Copy web assets to Android project
   cp index.html android/app/src/main/assets/
   
   # Open in Android Studio
   # File → Open → select 'android' folder
   ```

## 📋 Development Guidelines

### Code Style

#### HTML/CSS/JavaScript
- Use 2 spaces for indentation
- Use semantic HTML elements
- Follow BEM methodology for CSS classes
- Use modern JavaScript (ES6+)
- Comment complex logic
- Keep functions small and focused

#### Android (Java)
- Follow Android coding standards
- Use meaningful variable names
- Add JavaDoc comments for public methods
- Handle exceptions appropriately
- Follow Material Design guidelines

### Commit Messages
Use clear, descriptive commit messages:
```
feat: add episode bulk selection feature
fix: resolve localStorage issue on Safari
docs: update Android setup guide
style: improve button hover animations
refactor: simplify episode tracking logic
test: add unit tests for data export
```

### Branch Naming
- `feature/feature-name` - New features
- `fix/bug-description` - Bug fixes
- `docs/documentation-update` - Documentation changes
- `refactor/code-improvement` - Code refactoring
- `test/test-addition` - Adding tests

## 🐛 Reporting Issues

### Bug Reports
When reporting bugs, please include:

1. **Clear title** - Summarize the issue
2. **Description** - Detailed explanation of the problem
3. **Steps to reproduce** - How to recreate the issue
4. **Expected behavior** - What should happen
5. **Actual behavior** - What actually happens
6. **Environment details**:
   - Browser/version (for web issues)
   - Android version/device (for Android issues)
   - Operating system
7. **Screenshots** - If applicable
8. **Console errors** - Any error messages

### Feature Requests
For new features, please include:

1. **Clear title** - What feature you want
2. **Problem description** - What problem does this solve?
3. **Proposed solution** - How should it work?
4. **Alternatives considered** - Other approaches you thought of
5. **Additional context** - Screenshots, mockups, examples

## 💻 Code Contribution Process

### 1. Planning
- Check existing issues and PRs to avoid duplicates
- For major features, create an issue first to discuss
- Break large features into smaller, manageable PRs

### 2. Development
- Write clean, readable code
- Follow existing code patterns
- Add comments for complex logic
- Test your changes thoroughly

### 3. Testing
#### Web Testing
- Test in multiple browsers (Chrome, Firefox, Safari, Edge)
- Test on mobile devices
- Test PWA installation
- Verify offline functionality
- Test data import/export

#### Android Testing
- Test on different Android versions (API 21+)
- Test on different screen sizes
- Test file upload functionality
- Test WebView performance
- Verify permissions work correctly

### 4. Documentation
- Update README.md if needed
- Update relevant guide documents
- Add inline code comments
- Update version numbers if applicable

### 5. Pull Request
1. **Push your branch**
   ```bash
   git push origin feature/your-feature-name
   ```

2. **Create Pull Request**
   - Use a clear, descriptive title
   - Reference related issues (#123)
   - Describe what you changed and why
   - Include screenshots for UI changes
   - List any breaking changes

3. **PR Template**
   ```markdown
   ## Description
   Brief description of changes
   
   ## Type of Change
   - [ ] Bug fix
   - [ ] New feature
   - [ ] Documentation update
   - [ ] Refactoring
   
   ## Testing
   - [ ] Tested in Chrome
   - [ ] Tested in Firefox
   - [ ] Tested on mobile
   - [ ] Tested Android app (if applicable)
   
   ## Screenshots
   (if applicable)
   
   ## Related Issues
   Fixes #123
   ```

## 🎯 Priority Areas

We especially welcome contributions in these areas:

### High Priority
- 🐛 Bug fixes for reported issues
- 📱 Android app improvements
- ♿ Accessibility enhancements
- 🌐 Internationalization (i18n)
- 🔒 Security improvements

### Medium Priority
- 🎨 UI/UX improvements
- ⚡ Performance optimizations
- 📊 New analytics features
- 🔄 Data sync capabilities
- 🧪 Test coverage

### Low Priority
- 🎉 New themes
- 🔌 Third-party integrations
- 📈 Advanced statistics
- 🎮 Gamification features

## 🏗️ Project Structure

```
pop-watch-tracker/
├── index.html              # Main web app
├── README.md               # Project overview
├── LICENSE                 # MIT license
├── CONTRIBUTING.md         # This file
├── ANDROID_GUIDE.md        # Android development guide
├── ANDROID_SETUP.md        # Quick Android setup
├── android/                # Android app source
│   ├── app/
│   │   ├── src/main/
│   │   │   ├── java/       # Java source code
│   │   │   ├── res/        # Android resources
│   │   │   └── assets/     # Web assets
│   │   └── build.gradle    # App build config
│   ├── build.gradle        # Project build config
│   └── settings.gradle     # Project settings
└── docs/                   # Additional documentation
```

## 🔄 Review Process

1. **Automated checks** - GitHub Actions will run
2. **Code review** - Maintainers will review your code
3. **Testing** - Changes will be tested
4. **Feedback** - You may receive requests for changes
5. **Merge** - Approved PRs will be merged

## 🎉 Recognition

Contributors will be:
- Listed in the README.md contributors section
- Mentioned in release notes for significant contributions
- Given credit in commit messages and PR descriptions

## 📞 Getting Help

- **Questions**: Create a GitHub Discussion
- **Stuck**: Comment on your PR or issue
- **Ideas**: Start a Discussion thread
- **Direct contact**: saymynamejk0@gmail.com

## 📜 Code of Conduct

### Our Pledge
We pledge to make participation in our project a harassment-free experience for everyone, regardless of age, body size, disability, ethnicity, gender identity and expression, level of experience, nationality, personal appearance, race, religion, or sexual identity and orientation.

### Our Standards
- Use welcoming and inclusive language
- Be respectful of differing viewpoints
- Accept constructive criticism gracefully
- Focus on what's best for the community
- Show empathy towards other community members

### Enforcement
Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by contacting saymynamejk0@gmail.com.

## 🙏 Thank You

Every contribution, no matter how small, helps make Pop Watch Tracker better for everyone. Thank you for taking the time to contribute!

---

**Happy coding! 🚀**