# Publishing Guide for Trustworthy ML Website

This guide explains how to make changes and publish updates to your Trustworthy ML website at https://trustworthyml-ai.github.io/

## Prerequisites

- Git installed on your machine
- SSH key configured for GitHub (`~/.ssh/id_prashant_orion-ai_io`)
- Python with conda installed
- Access to the repository: `trustworthyml-ai/trustworthyml-ai.github.io`

## Directory Structure

```
/Users/prashantkulkarni/Documents/source-code/tml/
├── docs/                    # Source markdown files
│   ├── index.md            # Homepage
│   ├── about.md            # About page
│   ├── course/             # Course materials
│   ├── resources/          # Tools and datasets
│   └── research/           # Research papers
├── mkdocs.yml              # Site configuration
├── requirements.txt        # Python dependencies
└── site/                   # Built site (generated)
```

## Step-by-Step Publishing Procedure

### 1. Navigate to Project Directory

```bash
cd /Users/prashantkulkarni/Documents/source-code/tml
```

### 2. Activate Conda Environment

```bash
conda activate tml-site
```

If the environment doesn't exist, create it:
```bash
conda create -n tml-site python=3.11 -y
conda activate tml-site
pip install -r requirements.txt
```

### 3. Make Your Changes

Edit the appropriate markdown files in the `docs/` directory:

- **Homepage**: `docs/index.md`
- **About Page**: `docs/about.md`
- **Course Syllabus**: `docs/course/syllabus.md`
- **Course Schedule**: `docs/course/schedule.md`
- **Research Papers**: `docs/research/papers.md`
- **Tools**: `docs/resources/tools.md`
- **Datasets**: `docs/resources/datasets.md`

### 4. Preview Changes Locally (Optional)

```bash
mkdocs serve
```

Then visit http://localhost:8000 to preview your changes.

### 5. Build the Site

```bash
mkdocs build --clean
```

This creates/updates the `site/` directory with the built HTML files.

### 6. Copy Built Files to Root

Since we're using a special GitHub Pages setup, copy the built files to the root:

```bash
cp -r site/* .
```

### 7. Stage All Changes

```bash
git add .
```

### 8. Commit Changes

```bash
git commit -m "Your descriptive commit message

- Detail what you changed
- Why you made the changes
- Any relevant information"
```

### 9. Push to GitHub

```bash
git push
```

### 10. Verify Deployment

- Visit https://trustworthyml-ai.github.io/ 
- Changes should be live within 2-3 minutes
- Check GitHub Actions tab for deployment status

## Common Update Scenarios

### Adding a New Presentation

1. Edit `docs/about.md`
2. Find the "Featured Presentations" section
3. Add your presentation:

```markdown
**[Presentation Title](https://link-to-presentation)**  
*Conference Name* | Year  
Brief description of the talk content and key insights.
```

### Updating Course Information

1. Edit `docs/course/syllabus.md` for syllabus changes
2. Edit `docs/course/schedule.md` for schedule updates
3. Follow the build and publish steps above

### Adding Research Papers

1. Edit `docs/research/papers.md`
2. Add papers in the appropriate section:

```markdown
**[Paper Title](https://arxiv.org/link)** (Authors, Year)  
*Venue* | `tag1` `tag2`  
Brief description of the paper's contribution.
```

### Updating Tools or Datasets

1. Edit `docs/resources/tools.md` or `docs/resources/datasets.md`
2. Follow the existing format for consistency

## Troubleshooting

### Build Errors

If `mkdocs build` fails:
- Check for syntax errors in markdown files
- Ensure all internal links point to existing files
- Run `mkdocs build --strict` to see all warnings

### Push Rejected

If git push is rejected:
- Pull latest changes first: `git pull`
- Resolve any merge conflicts
- Commit and push again

### Site Not Updating

If changes aren't appearing:
- Clear browser cache
- Check GitHub Actions for deployment status
- Ensure you copied site files to root (`cp -r site/* .`)

## Quick Reference Commands

```bash
# Full publishing workflow
cd /Users/prashantkulkarni/Documents/source-code/tml
conda activate tml-site
mkdocs build --clean
cp -r site/* .
git add .
git commit -m "Update description"
git push
```

## Important Notes

- Always build with `mkdocs build --clean` to ensure fresh build
- The `cp -r site/* .` step is crucial - it copies built files to root
- GitHub Pages serves files from the repository root
- Changes typically appear online within 2-3 minutes

## Getting Help

- MkDocs Documentation: https://www.mkdocs.org/
- Material Theme Docs: https://squidfunk.github.io/mkdocs-material/
- GitHub Pages: https://docs.github.com/en/pages

---

Last updated: June 2025