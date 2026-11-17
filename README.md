# Learning Library Template

A reusable, blank, offline-first learning library web application.

Use this repository as a template for new learning libraries. The template includes module/topic navigation, a full-screen Markdown reader, KaTeX equation rendering, search, formula and glossary sections, bookmarks, completion tracking, progress indicators, light/dark themes, offline caching, and a GitHub Pages deployment workflow.

## Getting started
1. Create a new repository from this template.
2. Customize the title, description, theme, and navigation labels in `index.html`.
3. Add module and lesson records to `data/lectures-index.json`.
4. Add Markdown lessons under `lectures/module-XX/`.
5. Enable GitHub Pages using GitHub Actions.

## Index format
```json
{
  "version": 1,
  "modules": [{ "moduleNumber": 1, "title": "Module title", "description": "Short description" }],
  "topics": [{
    "id": "module-01-topic-01-01",
    "module": 1,
    "topicNumber": "1.1",
    "title": "Lesson title",
    "summary": "Short description",
    "path": "lectures/module-01/topic-01-01-lesson-title.md",
    "status": "complete"
  }]
}
```

This repository starts blank and contains no subject-specific lesson content.