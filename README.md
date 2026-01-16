# Trove

A curated collection of practical, hands-on resources for FHIR Terminology and SNOMED CT, compiled and created by Michael Osborne.

Trove is a playful reference to a comment made by a colleague who mentioned having access to "the most recent trove of exercises or related materials that could be reused/referenced for a Connectathon."

## Overview

This repository contains a documentation site built with MkDocs that serves as a central hub for FHIR terminology resources, SNOMED CT tools, and educational materials. It includes comprehensive glossaries, curated links to external resources, and personal contributions to the healthcare interoperability community.

## Key Topics

- **Expression Constraint Language (ECL)** - A formal language for defining precise, computable subsets of SNOMED CT clinical meanings
- **Intensional & Extensional Value Sets** - Different approaches to defining value sets in healthcare terminology
- **Terminology Servers** - Tools and techniques for managing and utilizing SNOMED CT and other code systems
- **FHIR Implementation** - Resources for implementing FHIR with proper terminology bindings
- **LOINC & SNOMED CT** - Standards for laboratory and clinical terminology

## Getting Started

### Prerequisites
- Python 3.7+
- pip

### Installation

1. Clone the repository:
```bash
git clone https://github.com/mjosborne1/trove.git
cd trove
```

2. Create a virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate
```

3. Install MkDocs:
```bash
pip install mkdocs mkdocs-theme-cinder
```

### Running Locally

To serve the documentation locally:
```bash
mkdocs serve
```

The site will be available at `http://localhost:8000`

### Building for Production

To build the static site:
```bash
mkdocs build
```

The output will be in the `site/` directory.

### Deploying to GitHub Pages

To deploy the site to GitHub Pages:
```bash
mkdocs gh-deploy
```

This command will:
1. Build the documentation
2. Push the site to the `gh-pages` branch
3. GitHub will automatically serve it at `https://mjosborne1.github.io/trove/`

**Note:** Ensure your repository is set up with GitHub Pages enabled on the `gh-pages` branch in your repository settings.

## Structure

```
trove/
├── docs/
│   ├── index.md          # Home page with glossary and resource links
│   ├── about.md          # About the author
│   └── favicon.svg       # Site icon (treasure chest)
├── mkdocs.yml            # MkDocs configuration
└── README.md             # This file
```

## About the Author

**Michael Osborne** is a healthcare terminology specialist with expertise in:
- SNOMED CT and LOINC standards
- FHIR Implementation Guides
- Terminology servers and interoperability
- Health information system development

He has been working with health terminology since the early 2000s and currently works at CSIRO AEHRC on terminology artifacts for FHIR Implementation Guides.

**Connect with Michael:**
- 📧 [Email](mailto:mjosborne1@gmail.com)
- 💼 [LinkedIn](https://www.linkedin.com/in/osbornemichael)
- 💬 [Zulip FHIR Chat](https://chat.fhir.org/#narrow/dm/192047-Michael-Osborne)

## License

This repository is provided as an educational resource for the healthcare interoperability community.

## Contributing

This is a curated personal resource collection. For questions, suggestions, or corrections, feel free to reach out to Michael via the contact methods listed above.
