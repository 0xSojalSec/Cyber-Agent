<div align="center">
  <img src="../public/hackgpt-logo.png" alt="HackGPT Enterprise Logo" width="250" height="auto">
</div>

# 🤝 Contributing to HackGPT Enterprise

Thank you for your interest in contributing to **HackGPT Enterprise**! This document provides guidelines for contributing to our AI-powered penetration testing platform.

## 🚀 Quick Start for Contributors

### Prerequisites
- **GitHub Account**: [Sign up here](https://github.com/join) if you don't have one
- **Git**: [Install Git](https://git-scm.com/downloads) on your system
- **Python 3.8+**: Required for development
- **Docker**: For containerized development (recommended)

### Development Setup
```bash
# Fork and clone the repository
git clone https://github.com/yourusername/HackGPT.git
cd HackGPT

# Set up development environment
chmod +x install.sh
./install.sh

# Create feature branch
git checkout -b feature/your-feature-name
```

## 🎯 How to Contribute

### 1. 🐛 Bug Reports
**Before submitting a bug report:**
- Check existing [issues](https://github.com/0xSojalSec/HackGPT/issues)
- Use the latest version of HackGPT
- Test in a clean environment

**When submitting:**
- Use the bug report template
- Include steps to reproduce
- Provide system information
- Attach logs or screenshots

### 2. 💡 Feature Requests
**For new features:**
- Check [discussions](https://github.com/0xSojalSec/HackGPT/discussions)
- Use the feature request template
- Explain the use case and benefits
- Consider security implications

### 3. 🔧 Code Contributions
**Pull Request Process:**
1. Fork the repository
2. Create a feature branch
3. Write code with tests
4. Ensure all tests pass
5. Submit pull request with clear description

**Code Standards:**
- Follow PEP 8 for Python
- Write comprehensive docstrings
- Include unit tests
- Update documentation

### 4. 📚 Documentation
**Help improve our documentation:**
- Fix typos or unclear explanations
- Add examples and tutorials
- Translate to other languages
- Update API documentation

## 🛡️ Security Contributions

### Vulnerability Reporting
**For security issues:**
- Email: yashabalam707@gmail.com
- Subject: "[SECURITY] HackGPT Vulnerability Report"
- Include detailed technical information
- Allow time for responsible disclosure

### Security Feature Development
**When adding security features:**
- Follow OWASP guidelines
- Consider privacy implications
- Include threat modeling
- Add security tests

## 💰 Financial Contributions

### Individual Supporters
Support HackGPT development through:
- **GitHub Sponsors**: [Sponsor Yashab Alam](https://github.com/sponsors/0xSojalSec)
- **PayPal**: [paypal.me/yashab07](https://paypal.me/yashab07)
- **Cryptocurrency**: See [DONATE.md](../DONATE.md) for addresses

### Corporate Sponsorship
**For companies interested in sponsoring:**
- **Email**: yashabalam707@gmail.com
- **Subject**: "HackGPT Enterprise Sponsorship Inquiry"
- **Include**: Company info, sponsorship goals, budget range

**Sponsorship Benefits:**
- 🏢 Logo placement in README and documentation
- 📢 Announcement on social media channels
- 🤝 Direct communication with development team
- 🎯 Feature development priority
- 📈 Usage analytics and reports

## 👥 Community Guidelines

### Communication Channels
- **GitHub Issues**: Bug reports and feature requests
- **GitHub Discussions**: General questions and ideas
- **WhatsApp Business**: [Join Channel](https://whatsapp.com/channel/0029Vaoa1GfKLaHlL0Kc8k1q)
- **Email**: yashabalam707@gmail.com

### Code of Conduct
Please read our [Code of Conduct](CODE_OF_CONDUCT.md) before participating. We're committed to maintaining a welcoming, inclusive, and secure community.

## 🏷️ Issue and PR Templates

### Bug Report Template
```markdown
**Bug Description**
A clear and concise description of what the bug is.

**To Reproduce**
Steps to reproduce the behavior:
1. Go to '...'
2. Click on '....'
3. Scroll down to '....'
4. See error

**Expected Behavior**
A clear and concise description of what you expected to happen.

**Screenshots**
If applicable, add screenshots to help explain your problem.

**Environment:**
 - OS: [e.g. Ubuntu 20.04]
 - Python Version: [e.g. 3.9]
 - HackGPT Version: [e.g. 2.0.0]

**Additional Context**
Add any other context about the problem here.
```

### Feature Request Template
```markdown
**Is your feature request related to a problem?**
A clear and concise description of what the problem is.

**Describe the solution you'd like**
A clear and concise description of what you want to happen.

**Describe alternatives you've considered**
A clear and concise description of any alternative solutions.

**Use Case**
Explain how this feature would be used in practice.

**Security Considerations**
Any security implications of this feature.

**Additional Context**
Add any other context or screenshots about the feature request here.
```

## 🎖️ Recognition

### Contributors
All contributors are recognized in:
- **CONTRIBUTORS.md**: List of all project contributors
- **GitHub Contributors**: Automatic recognition by GitHub
- **Release Notes**: Major contributors mentioned in releases
- **Social Media**: Contributors highlighted on ZehraSec social channels

### Sponsorship Recognition
- **Bronze Sponsors ($5-24)**: Name in CONTRIBUTORS.md
- **Silver Sponsors ($25-99)**: Logo in README.md
- **Gold Sponsors ($100-499)**: Logo in documentation
- **Platinum Sponsors ($500+)**: Premium placement and announcements

## 🔄 Development Workflow

### Branch Strategy
```bash
main                 # Stable production code
├── develop         # Integration branch for features
├── feature/*       # New features
├── bugfix/*        # Bug fixes
├── hotfix/*        # Critical production fixes
└── release/*       # Release preparation
```

### Commit Message Convention
```
type(scope): description

[optional body]

[optional footer]
```

**Types**: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`

**Examples:**
```bash
feat(ai): add GPT-4 integration for vulnerability analysis
fix(scanner): resolve Nmap output parsing issue
docs(readme): update installation instructions
```

## 🧪 Testing Guidelines

### Running Tests
```bash
# Unit tests
pytest tests/unit/

# Integration tests
pytest tests/integration/

# Security tests
bandit -r .
safety check

# All tests
pytest
```

### Writing Tests
- Write tests for all new features
- Ensure tests are deterministic
- Mock external dependencies
- Include edge cases
- Test security features thoroughly

## 📦 Release Process

### Version Numbering
We follow [Semantic Versioning](https://semver.org/):
- **MAJOR**: Incompatible API changes
- **MINOR**: Backwards-compatible functionality
- **PATCH**: Backwards-compatible bug fixes

### Release Checklist
- [ ] All tests passing
- [ ] Documentation updated
- [ ] CHANGELOG.md updated
- [ ] Version numbers updated
- [ ] Security scan completed
- [ ] Docker images built and tested

## 🌐 Internationalization

### Adding Translations
- Create language files in `locales/`
- Use standard ISO language codes
- Test with right-to-left languages
- Update documentation in multiple languages

### Supported Languages
Currently seeking translators for:
- Spanish (es)
- French (fr) 
- German (de)
- Chinese (zh)
- Japanese (ja)
- Russian (ru)

## 📞 Getting Help

### For Contributors
- **Technical Questions**: [GitHub Discussions](https://github.com/0xSojalSec/HackGPT/discussions)
- **Development Help**: yashabalam707@gmail.com
- **Real-time Chat**: [WhatsApp Business Channel](https://whatsapp.com/channel/0029Vaoa1GfKLaHlL0Kc8k1q)

### For Sponsors/Investors
- **Partnership Inquiries**: yashabalam707@gmail.com
- **Corporate Sponsorship**: Include "SPONSORSHIP" in subject line
- **Investment Opportunities**: Include "INVESTMENT" in subject line
- **LinkedIn**: [Yashab Alam](https://www.linkedin.com/in/yashab-alam)

## 🏢 About ZehraSec

**ZehraSec** is a cybersecurity research and development company founded by Yashab Alam, focused on advancing AI-powered security solutions.

**Connect with ZehraSec:**
- 🌐 **Website**: [www.zehrasec.com](https://www.zehrasec.com)
- 📸 **Instagram**: [@_zehrasec](https://www.instagram.com/_zehrasec)
- 💼 **LinkedIn**: [ZehraSec Company](https://www.linkedin.com/company/zehrasec)
- 🐦 **Twitter**: [@zehrasec](https://x.com/zehrasec)

---

**Thank you for contributing to HackGPT Enterprise! Together, we're building the future of AI-powered cybersecurity.**

*Made with ❤️ by the HackGPT Enterprise community*
