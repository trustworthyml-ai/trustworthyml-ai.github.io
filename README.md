# Trustworthy Machine Learning Resource Hub

[![Deploy MkDocs](https://github.com/trustworthyml-ai/trustworthyml-ai/actions/workflows/deploy.yml/badge.svg)](https://github.com/trustworthyml-ai/trustworthyml-ai/actions/workflows/deploy.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> A comprehensive resource hub for **Trustworthy Machine Learning** - course materials, research papers, tools, and community resources.

🌐 **Live Site**: [https://trustworthyml-ai.github.io/](https://trustworthyml-ai.github.io/)

## About

This repository contains the source code for the Trustworthy ML resource website, built with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/). The site serves as a comprehensive hub for:

- 📚 **Course Materials**: Syllabus, assignments, and projects for Fall 2024 TML course
- 📑 **Research Library**: Curated collection of key papers in trustworthy ML
- 🛠️ **Tools & Resources**: Comprehensive toolkit for practitioners
- 👥 **Community**: Discussion forums, events, and contribution guidelines

## Quick Start

### Prerequisites

- Python 3.8+
- Git

### Local Development

```bash
# Clone the repository
git clone https://github.com/trustworthyml-ai/trustworthyml-ai.git
cd trustworthyml-ai

# Install dependencies
pip install -r requirements.txt

# Serve locally
mkdocs serve
```

Visit [http://localhost:8000](http://localhost:8000) to view the site.

### Building for Production

```bash
mkdocs build
```

The built site will be in the `site/` directory.

## Site Structure

```
docs/
├── index.md                 # Homepage
├── course/                  # Course materials
│   ├── syllabus.md         # Course syllabus
│   ├── schedule.md         # Lecture schedule
│   ├── assignments.md      # Assignment details
│   └── projects.md         # Project guidelines
├── resources/              # Tools and resources
│   ├── tools.md           # Software tools
│   ├── datasets.md        # Benchmark datasets
│   └── tutorials.md       # Tutorials and guides
├── research/               # Research papers
│   ├── papers.md          # Paper library
│   ├── topics.md          # Key research topics
│   └── recent.md          # Recent advances
└── community/              # Community resources
    ├── discussion.md       # Discussion forums
    ├── events.md          # Upcoming events
    └── contributing.md    # Contribution guide
```

## Key Features

### 🎨 Modern Design
- **Material Design**: Clean, responsive interface
- **Dark/Light Theme**: Toggle between themes
- **Mobile Optimized**: Works perfectly on all devices

### 🔍 Enhanced Search
- **Full-text Search**: Search across all content
- **Syntax Highlighting**: Code examples with highlighting
- **Navigation**: Tabbed navigation with breadcrumbs

### 📊 Rich Content
- **Interactive Examples**: Code snippets with copy buttons
- **Admonitions**: Notes, tips, warnings, and more
- **Tables**: Sortable comparison tables
- **Tags**: Categorized content with filtering

### 🚀 Automated Deployment
- **GitHub Actions**: Automatic deployment on push
- **GitHub Pages**: Free hosting with custom domain support
- **Performance**: Optimized builds with minification

## Contributing

We welcome contributions from the community! See our [Contributing Guide](docs/community/contributing.md) for details on:

- Adding new papers to the research library
- Contributing tool reviews and tutorials
- Improving course materials
- Reporting bugs and suggesting features

### Quick Contribution

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add amazing feature'`)
5. Push to the branch (`git push origin feature/amazing-feature`)
6. Open a Pull Request

## Course Information

**Trustworthy Machine Learning - Fall 2024**

This course provides comprehensive coverage of trustworthy ML principles including:

- **Fairness & Bias**: Detection, measurement, and mitigation
- **Robustness**: Adversarial examples and certified defenses  
- **Interpretability**: Explanation methods and evaluation
- **Privacy**: Differential privacy and federated learning
- **Safety**: AI alignment and verification

See the [full syllabus](docs/course/syllabus.md) for detailed information.

## Technology Stack

- **[MkDocs](https://www.mkdocs.org/)**: Static site generator
- **[Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)**: Theme and components
- **[GitHub Pages](https://pages.github.com/)**: Hosting platform
- **[GitHub Actions](https://github.com/features/actions)**: CI/CD pipeline

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Course materials inspired by leading TML research
- Community contributions from students and researchers
- Tools and frameworks from the open-source community

## Contact

- **Issues**: [GitHub Issues](https://github.com/trustworthyml-ai/trustworthyml-ai/issues)
- **Discussions**: [GitHub Discussions](https://github.com/trustworthyml-ai/trustworthyml-ai/discussions)

---

⭐ **Star this repository** if you find it helpful! It helps others discover this resource.
