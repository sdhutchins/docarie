# Docarie

A tasteful assortment of accessible and comprehensive documentation for bioinformatics tools and computational biology workflows.

View [docarie](https://www.shauritahutchins.com/docarie/).

## About

Docarie provides comprehensive guides, tutorials, and reference materials to help researchers and developers work effectively with various computational biology tools. This site focuses on making complex bioinformatics workflows accessible through clear, well-structured documentation.

### Currently Available

- **MERLIN Tutorials** - Complete documentation for genetic linkage analysis, including: parametric and non-parametric linkage analysis, association analysis, IBD estimation, haplotyping, error detection, WGS preprocessing, and genetic map integration.

## Quick Start

```bash
# Install Quarto (if not already installed)
# https://quarto.org/docs/get-started/

# Clone and preview the site
git clone https://github.com/sdhutchins/docarie.git
cd docarie
quarto preview
```

## Project Structure

```
docarie/
├── _quarto.yml          # Site configuration
├── index.qmd            # Home page
├── assets/              # Stylesheets and static files
├── docs/
│   └── merlin/          # MERLIN documentation
│       ├── index.qmd    # Tutorial overview
│       ├── parametric.qmd
│       ├── linkage.qmd
│       ├── notes.qmd    # WGS preprocessing guide
│       └── ...          # Additional tutorials
└── _site/               # Generated site (auto-created)
```

## Contributing

### Adding New Tool Documentation

1. Create a new directory: `docs/toolname/`
2. Add navigation in `_quarto.yml`:
   ```yaml
   navbar:
     left:
       - href: docs/toolname/
         text: ToolName
   ```
3. Create `index.qmd` and tutorial files
4. Follow the established markdown formatting patterns

### Content Guidelines

- Use clear, step-by-step instructions
- Include command examples with proper syntax highlighting
- Provide context and background for each tool/method
- Cross-reference related tutorials where applicable

## Author

**Shaurita D. Hutchins** | Graduate Research Assistant | [@sdhutchins](https://github.com/sdhutchins)

## Resources

- [Quarto Documentation](https://quarto.org/docs/)
- [Quarto Websites Guide](https://quarto.org/docs/websites/)
- [MERLIN Software](https://csg.sph.umich.edu/abecasis/merlin/)

## License

This documentation is available under the [MIT License](LICENSE). 