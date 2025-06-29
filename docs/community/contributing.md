# Contributing to Trustworthy ML

We welcome contributions from the community! Whether you're a student, researcher, or practitioner, there are many ways to help build the most comprehensive resource for trustworthy machine learning.

## Ways to Contribute

### 📚 Content Contributions

**Research Papers**
- Submit new papers to our [research library](../research/papers.md)
- Add summaries and practical insights to existing papers
- Suggest paper categorizations and tags

**Tools & Resources**
- Add new tools to our [toolkit collection](../resources/tools.md)
- Update installation instructions and compatibility info
- Share usage examples and best practices

**Course Materials**
- Contribute assignment ideas and solutions
- Share project examples and case studies
- Suggest improvements to course structure

### 🐛 Issue Reports

Found something wrong? [Open an issue](https://github.com/trustworthyml-ai/trustworthyml-ai/issues) for:

- Broken links or outdated information
- Technical errors in code examples
- Missing important papers or tools
- Suggestions for new content sections

### 💡 Feature Requests

Help us improve the site by suggesting:

- New sections or content types
- Interactive tutorials or demos
- Community features (forums, events)
- Integration with external tools

## Contribution Guidelines

### Content Standards

**Quality Requirements**
- ✅ Accurate and up-to-date information
- ✅ Clear, concise writing appropriate for academic audience
- ✅ Proper citations and attribution
- ✅ Reproducible code examples where applicable

**Paper Submissions**
- Must be peer-reviewed publications or high-quality preprints
- Include full citation with venue and year
- Add 2-3 sentence summary of significance
- Tag with relevant topics using our taxonomy

**Tool Reviews**
- Test installation and basic functionality
- Include clear installation instructions
- Rate usability (⭐ to ⭐⭐⭐⭐⭐)
- Mention integration with other tools

### Style Guide

**Markdown Formatting**
```markdown
# Main Headings (H1)
## Section Headings (H2)
### Subsection Headings (H3)

**Bold** for emphasis
*Italics* for paper titles
`code` for inline code
```

**Paper References**
```markdown
**[Paper Title](link)** (Authors, Year)  
*Venue* | `tag1` `tag2` `tag3`  
Brief description of contribution and significance.
```

**Tool Listings**
```markdown
**[Tool Name](link)**  
*Organization* | Language | ⭐⭐⭐⭐  
```bash
pip install tool-name
```
- **Features**: Key capabilities
- **Best for**: Primary use cases
- **Integration**: Compatible frameworks
```

### Pull Request Process

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/add-new-paper`)
3. **Make** your changes following our style guide
4. **Test** any code examples
5. **Commit** with descriptive messages
6. **Submit** a pull request with:
   - Clear description of changes
   - Link to any relevant issues
   - Screenshots for UI changes

### Review Process

All contributions go through peer review:

1. **Automated checks**: Formatting, links, builds
2. **Content review**: Accuracy, relevance, quality
3. **Technical review**: Code functionality, reproducibility
4. **Final approval**: Maintainer approval for merge

Typical review time: 3-7 days for content, 1-3 days for fixes.

## Recognition

Contributors are recognized in multiple ways:

### Git Attribution
All contributions are tracked in git history with proper attribution.

### Contributors Page
Regular contributors are featured on our [contributors page](contributors.md) with:
- Profile and bio
- Areas of expertise
- Contributions summary

### Academic Citation
For significant contributions (new sections, major tool reviews):
- Co-authorship consideration on related publications
- Citation in academic papers referencing this resource

## Community Guidelines

### Code of Conduct

We are committed to providing a welcoming and inclusive environment:

- ✅ **Be respectful** in all interactions
- ✅ **Assume good intentions** from contributors
- ✅ **Provide constructive feedback** on contributions
- ✅ **Credit others' work** appropriately
- ❌ **No harassment or discrimination** of any kind
- ❌ **No spam or self-promotion** without value

### Communication Channels

- **GitHub Issues**: Bug reports, feature requests
- **Discussions**: General questions, ideas, community chat
- **Email**: [contact@trustworthyml.ai](mailto:contact@trustworthyml.ai)

### Response Times

We aim to respond to:
- **Issues**: Within 48 hours
- **Pull requests**: Within 1 week
- **Questions**: Within 24 hours

## Getting Started

### New Contributors

1. **Read** the [README](https://github.com/trustworthyml-ai/trustworthyml-ai/blob/main/README.md)
2. **Browse** [good first issues](https://github.com/trustworthyml-ai/trustworthyml-ai/labels/good%20first%20issue)
3. **Join** our [discussion forum](https://github.com/trustworthyml-ai/trustworthyml-ai/discussions)
4. **Introduce yourself** and ask questions!

### Quick Contributions

Easy ways to start contributing:

- **Fix typos** or broken links
- **Add missing citations** to paper references  
- **Update installation instructions** for tools
- **Add tags** to untagged content
- **Share usage examples** for existing tools

### Substantial Contributions

For larger contributions:

1. **Open an issue** to discuss your idea first
2. **Get feedback** from maintainers and community
3. **Plan your approach** with milestones
4. **Submit incremental PRs** for review

## Technical Setup

### Local Development

```bash
# Clone the repository
git clone https://github.com/trustworthyml-ai/trustworthyml-ai.git
cd trustworthyml-ai

# Install MkDocs and dependencies
pip install mkdocs-material
pip install mkdocs-git-revision-date-localized-plugin

# Serve locally
mkdocs serve
```

Visit `http://localhost:8000` to preview your changes.

### Dependencies

The site uses:
- **MkDocs**: Static site generator
- **Material theme**: Modern, responsive design
- **Git plugins**: Automatic timestamps and contributors
- **GitHub Actions**: Automated deployment

---

## Questions?

**Need help getting started?**  
Check our [FAQ](faq.md) or [open a discussion](https://github.com/trustworthyml-ai/trustworthyml-ai/discussions).

**Found a bug or security issue?**  
Please report it via [GitHub Issues](https://github.com/trustworthyml-ai/trustworthyml-ai/issues) or email us directly for security concerns.

Thank you for helping build the trustworthy ML community! 🚀