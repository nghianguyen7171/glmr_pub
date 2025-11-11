# GlennMurray Published (GLMR)

GlennMurray Published (GLMR) is an Elsevier-inspired journal site that curates the 2025 Introduction to AI midterm presentations and reports. The site is generated from Markdown and served through GitHub Pages under `docs/`, making it easy to publish lecture notes and student work with minimal setup.

## Live Site
- **Homepage:** https://nghianguyen7171.github.io/glmr_pub/
- **Current Issue:** https://nghianguyen7171.github.io/glmr_pub/issue-1.html
- **Scoring Summary:** https://nghianguyen7171.github.io/glmr_pub/scoring-summary.html

## Features
- Professional hero/section styling inspired by Elsevier journals.
- Issue catalogue with English article titles, inline PDF reading, and download links.
- Detailed article pages per report containing authorship, scores, highlights, and instructor feedback.
- Presentation deck library with alternate exports.
- Markdown-driven content that can be edited without touching HTML.

## Repository Structure
```
GLMR_Publish/
├── docs/                    # GitHub Pages source
│   ├── index.md             # Home page
│   ├── issue-1.md           # Current issue overview
│   ├── scoring-summary.md   # Combined presentation/report scores
│   ├── _layouts/            # Custom layouts (journal & article)
│   ├── _includes/           # Shared head snippets (fonts, favicon)
│   └── assets/              # Custom CSS, favicon, etc.
├── Midterm_AI_Project/      # Submitted reports (PDF + extracted text)
├── Midterm_presentation/    # Presentation decks
├── presentation_raking.csv  # Original presentation ranking data
├── backup-context.md        # Session change log & instructions
└── README.md                # This file
```

## Local Preview
The site uses standard Jekyll-compatible markdown. To preview locally:

```bash
# Install dependencies (one time, requires Ruby)
gem install bundler jekyll

# Serve the docs/ directory
jekyll serve --source docs --baseurl ""

# Visit http://localhost:4000/ in your browser
```

> Note: If you prefer a minimal preview, any Markdown-aware static server can be used, but the hero styling assumes GitHub Pages’ Jekyll pipeline.

## Publishing Workflow
1. Commit changes to the repository.
2. Push to `main` – GitHub Pages is already configured to deploy from `docs/`.
3. Wait for the Pages build (typically < 1 minute) and refresh the public URL.

## Adding a New Issue
1. Duplicate `docs/issue-1.md` to `docs/issue-<n>.md` and update hero metadata, cards, and links.
2. Create accompanying article pages under `docs/articles/` following the existing front matter structure.
3. Update navigation in `docs/index.md` and `docs/_layouts/journal.html` if necessary.
4. Update `backup-context.md` with the latest change log and timestamp.

## Contributing
- Follow the styling conventions in `docs/assets/css/journal.css` when introducing new components.
- Keep report and presentation filenames ASCII-only to maintain compatibility with raw GitHub URLs.
- Use descriptive commit messages and update `backup-context.md` at the end of each session.

## License
Project artifacts are intended for academic reference within the Introduction to AI course. Consult the course instructor before reusing materials outside the class.
