# Contributing to Pop Watch Tracker 🤝

Thank you for your interest in contributing to Pop Watch Tracker! This document provides guidelines and information for contributors.

## 🌟 Ways to Contribute

### 🐛 Bug Reports
- Check [existing issues](https://github.com/yourusername/pop-watch-tracker/issues) first
- Use the bug report template
- Include browser/device information
- Provide steps to reproduce

### 💡 Feature Requests
- Check if the feature already exists or is planned
- Use the feature request template
- Explain the use case and benefits
- Consider implementation complexity

### 📝 Code Contributions
- Fork the repository
- Create a feature branch
- Follow coding standards
- Test your changes thoroughly
- Submit a pull request

### 📚 Documentation
- Improve README.md
- Add code comments
- Create tutorials or guides
- Fix typos and grammar

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome 80+, Firefox 75+, Safari 13+, Edge 80+)
- Basic knowledge of HTML, CSS, and JavaScript
- Git for version control

### Development Setup
```bash
# 1. Fork the repository on GitHub
# 2. Clone your fork locally
git clone https://github.com/yourusername/pop-watch-tracker.git
cd pop-watch-tracker

# 3. Create a feature branch
git checkout -b feature/your-feature-name

# 4. Make your changes
# Edit files using your preferred editor

# 5. Test locally
# Open index.html in your browser
# Test on different screen sizes
# Verify PWA functionality

# 6. Commit your changes
git add .
git commit -m "feat: add your feature description"

# 7. Push to your fork
git push origin feature/your-feature-name

# 8. Create a Pull Request on GitHub
```

## 📋 Coding Standards

### HTML
- Use semantic HTML5 elements
- Include proper ARIA labels for accessibility
- Maintain proper indentation (2 spaces)
- Use meaningful class and ID names

### CSS
- Follow BEM methodology for class naming
- Use CSS custom properties (variables)
- Mobile-first responsive design
- Maintain consistent spacing and typography

### JavaScript
- Use ES6+ features
- Follow functional programming principles
- Add JSDoc comments for functions
- Handle errors gracefully
- Use meaningful variable names

### Code Style
```javascript
// ✅ Good
function calculateProgress(show) {
  if (!show || !show.seasons) return 0;
  
  const totalEpisodes = show.seasons.reduce((total, season) => {
    return total + (season.episodes ? season.episodes.length : 0);
  }, 0);
  
  const watchedEpisodes = show.seasons.reduce((total, season) => {
    return total + (season.episodes ? season.episodes.filter(ep => ep.watched).length : 0);
  }, 0);
  
  return totalEpisodes > 0 ? (watchedEpisodes / totalEpisodes) * 100 : 0;
}

// ❌ Avoid
function calc(s) {
  var t = 0, w = 0;
  for(var i = 0; i < s.seasons.length; i++) {
    t += s.seasons[i].episodes.length;
    for(var j = 0; j < s.seasons[i].episodes.length; j++) {
      if(s.seasons[i].episodes[j].watched) w++;
    }
  }
  return t > 0 ? (w/t)*100 : 0;
}
```

## 🧪 Testing Guidelines

### Manual Testing Checklist
- [ ] Test on multiple browsers (Chrome, Firefox, Safari, Edge)
- [ ] Test responsive design (mobile, tablet, desktop)
- [ ] Test PWA installation and offline functionality
- [ ] Test accessibility with keyboard navigation
- [ ] Test dark/light theme switching
- [ ] Test data export/import functionality
- [ ] Test all CRUD operations (Create, Read, Update, Delete)

### Testing New Features
1. **Functionality**: Does the feature work as expected?
2. **UI/UX**: Is the interface intuitive and accessible?
3. **Performance**: Does it impact app performance?
4. **Compatibility**: Works across supported browsers?
5. **Data Integrity**: Doesn't corrupt existing data?

## 📝 Commit Message Guidelines

Use conventional commit format:

```
type(scope): description

[optional body]

[optional footer]
```

### Types
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes (formatting, etc.)
- `refactor`: Code refactoring
- `test`: Adding or updating tests
- `chore`: Maintenance tasks

### Examples
```bash
feat(episodes): add bulk episode marking functionality
fix(search): resolve case-sensitive search issue
docs(readme): update installation instructions
style(css): improve button hover animations
refactor(storage): optimize data persistence logic
```

## 🔍 Pull Request Process

### Before Submitting
1. **Test thoroughly** on multiple browsers
2. **Update documentation** if needed
3. **Check for conflicts** with main branch
4. **Follow coding standards**
5. **Write clear commit messages**

### PR Template
```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Performance improvement
- [ ] Code refactoring

## Testing
- [ ] Tested on Chrome
- [ ] Tested on Firefox
- [ ] Tested on mobile
- [ ] Tested PWA functionality

## Screenshots (if applicable)
Add screenshots for UI changes

## Additional Notes
Any additional information or context
```

### Review Process
1. **Automated checks** (if any) must pass
2. **Code review** by maintainers
3. **Testing** by reviewers
4. **Approval** and merge

## 🎯 Feature Development Guidelines

### Planning New Features
1. **Create an issue** first to discuss the feature
2. **Consider user impact** and use cases
3. **Plan implementation** approach
4. **Consider accessibility** requirements
5. **Think about mobile** experience

### Implementation Best Practices
- **Start small**: Implement MVP first
- **Progressive enhancement**: Ensure basic functionality works everywhere
- **Accessibility first**: Include ARIA labels and keyboard support
- **Performance conscious**: Minimize impact on app performance
- **Data backward compatibility**: Don't break existing user data

## 🐛 Bug Fix Guidelines

### Investigating Bugs
1. **Reproduce the issue** consistently
2. **Identify root cause** through debugging
3. **Consider edge cases** and side effects
4. **Test the fix** thoroughly
5. **Verify no regression** in other features

### Bug Fix Checklist
- [ ] Issue reproduced and understood
- [ ] Root cause identified
- [ ] Fix implemented and tested
- [ ] No regression in existing functionality
- [ ] Edge cases considered
- [ ] Documentation updated if needed

## 📱 PWA Development Notes

### Service Worker Updates
- Test offline functionality
- Verify cache invalidation
- Test app updates and refresh

### Manifest Changes
- Validate manifest.json syntax
- Test installation flow
- Verify icons and metadata

## 🎨 Design Guidelines

### Visual Consistency
- Follow existing design patterns
- Use established color palette
- Maintain consistent spacing
- Follow typography hierarchy

### Accessibility
- Minimum contrast ratios (WCAG AA)
- Keyboard navigation support
- Screen reader compatibility
- Touch target sizes (44px minimum)

## 📞 Getting Help

### Resources
- **Documentation**: Check README.md and code comments
- **Issues**: Search existing GitHub issues
- **Discussions**: Use GitHub Discussions for questions
- **Email**: Contact saymynamejk0@gmail.com for complex issues

### Communication
- **Be respectful** and constructive
- **Provide context** when asking questions
- **Share relevant information** (browser, OS, steps taken)
- **Be patient** - maintainers are volunteers

## 🏆 Recognition

Contributors will be recognized in:
- README.md contributors section
- Release notes for significant contributions
- GitHub contributors graph

## 📋 Issue Templates

### Bug Report Template
```markdown
**Describe the bug**
A clear description of what the bug is.

**To Reproduce**
Steps to reproduce the behavior:
1. Go to '...'
2. Click on '....'
3. Scroll down to '....'
4. See error

**Expected behavior**
What you expected to happen.

**Screenshots**
If applicable, add screenshots.

**Environment:**
- Browser: [e.g. Chrome 91]
- OS: [e.g. Windows 10]
- Device: [e.g. iPhone 12]
- App Version: [e.g. 2.5.0]
```

### Feature Request Template
```markdown
**Is your feature request related to a problem?**
A clear description of what the problem is.

**Describe the solution you'd like**
A clear description of what you want to happen.

**Describe alternatives you've considered**
Alternative solutions or features you've considered.

**Additional context**
Any other context or screenshots about the feature request.
```

Thank you for contributing to Pop Watch Tracker! 🍿✨