# Contributing to zsel-catalog

Thank you for contributing educational content to ZSEL!

## Getting Started

1. **Fork** the repository
2. **Clone** your fork
3. **Create a branch**: `git checkout -b content/course-name`
4. **Add content** following guidelines
5. **Submit pull request**

## Content Guidelines

### Course Structure
```
course-name/
├── README.md             Course overview
├── syllabus.md          Course syllabus and goals
├── modules/
│   ├── module-1/
│   │   ├── README.md
│   │   ├── lessons.md
│   │   └── assignments.md
│   └── module-2/
└── resources.md          Course resources
```

### File Organization
- Use clear, descriptive names
- Organize by module/topic
- Group related content
- Maintain consistent structure

### Metadata

Every course must include:
```
---
title: Course Name
author: Your Name
date: 2026-03-11
version: 1.0
learning_objectives: [...] 
keywords: [...]
---
```

## Content Standards

### Writing
- Be clear and concise
- Use active voice
- Include examples
- Proofread carefully
- Avoid jargon where possible

### Assignments
- Include clear instructions
- Define learning objectives
- Provide grading rubric
- Offer example solution
- Set realistic timeline

### Resources
- Link to primary sources
- Verify all links work
- Include access instructions
- Note any access restrictions
- Credit original authors

## Licensing

All content must declare license:
- **CC-BY-SA**: Content you created
- **CC-BY**: Content others created (attribute)
- **Proprietary**: Restricted to ZSEL only
- **Permission**: Explicit permission from owner

Include license in metadata:
```
---
license: CC-BY-SA
copyright_holder: Your Name
license_url: https://creativecommons.org/licenses/by-sa/4.0/
---
```

## Large Files (Video, Images)

Use Git LFS for files > 10MB:
```bash
git lfs track "*.mp4"
git lfs track "*.psd"
git add .gitattributes

# Then commit videos normally
git add videos/lecture.mp4
git commit -m "Add lecture video"
```

## Accessibility

Ensure content is accessible:
- [ ] Use alt text for images
- [ ] Include captions for videos
- [ ] Use clear fonts
- [ ] Provide transcripts
- [ ] Use color + symbols (not just color)

## Quality Checklist

Before submitting:
- [ ] Metadata complete
- [ ] Files properly organized
- [ ] All links verified
- [ ] Grammar/spelling checked
- [ ] Licensing declared
- [ ] Accessibility reviewed
- [ ] Example solutions included
- [ ] Rubrics clear and specific

## Updating Existing Content

To improve existing content:
1. Create branch from current content
2. Make improvements
3. Document what changed
4. Note version update
5. Submit PR with rationale

## Removing Content

To deprecate content:
1. Mark as deprecated in metadata
2. Suggest replacement
3. Set removal date
4. Migrate students to new content
5. Archive old content

## Reviews

Content reviewers check:
- [ ] Accuracy of information
- [ ] Appropriateness for grade level
- [ ] Clarity of instructions
- [ ] Quality of resources
- [ ] Proper licensing
- [ ] Accessibility compliance

## Questions?

- **Guidelines**: See [docs/ORGANIZATION.md](docs/ORGANIZATION.md)
- **Licensing**: See [docs/LICENSING.md](docs/LICENSING.md)
- **Help**: content-team@zsel.opole.pl

---

Thank you for creating great content! 📚✨
