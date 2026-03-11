# zsel-catalog: Educational Content Catalog

**Purpose**: Central repository for student educational content - courses, resources, assignments, media library

**Part of**: [ZSEL 7-Layer Architecture](../SERWERY/docs/ARCHITECTURE.md)

## Overview

The Content Catalog (zsel-catalog) manages:
- **Courses**: Course materials, syllabus, learning objectives
- **Resources**: Books, articles, videos, reference materials
- **Assignments**: Assignment descriptions, rubrics, exemplars
- **Media**: Images, videos, documents, presentations

## Directory Structure

```
zsel-catalog/
├── courses/
│   ├── 2a-fundamentals/     Fundamentals course materials
│   ├── 2b-intermediate/     Intermediate course materials
│   ├── 3a-advanced/         Advanced course materials
│   └── 3b-specialization/   Specialization courses
├── resources/
│   ├── textbooks/           Textbook PDFs and references
│   ├── articles/            Journal articles and papers
│   ├── videos/              Video tutorials and lectures
│   └── code-samples/        Code examples and templates
├── assignments/
│   ├── rubrics/             Grading rubrics
│   ├── templates/           Assignment templates
│   └── exemplars/           Example solutions
├── media/
│   ├── images/              Course images (Git LFS)
│   ├── videos/              Course videos (Git LFS)
│   └── documents/           Supporting documents
├── docs/
│   ├── ORGANIZATION.md      Content organization standards
│   ├── LICENSING.md         Copyright and licensing info
│   └── SUBMISSION.md        Content submission procedures
└── README.md
```

## Course Organization

### Course Codes
- **2a-fundamentals**: Grade 2 fundamentals
- **2b-intermediate**: Grade 2 intermediate
- **3a-advanced**: Grade 3 advanced
- **3b-specialization**: Grade 3 specialization

### Course Contents
Each course includes:
```
course-name/
├── syllabus.md              Course overview and goals
├── modules/
│   ├── module-1/
│   │   ├── README.md        Module overview
│   │   ├── lessons/         Individual lessons
│   │   └── assignments/     Module assignments
│   └── module-2/
├── resources/               Course-specific resources
└── assessments.md           Assessment procedures
```

## Resources Library

### Video Resources (Git LFS)
- Course lectures
- Tutorial videos
- Demonstration videos
- Guest lectures

### Textbook Materials
- Core textbooks
- Reference books
- Supplementary reading
- Research papers

### Code Samples
- Language examples
- Framework tutorials
- Best practices
- Common patterns

## Assignments

### Rubric Format
```
Assignment Name
Learning Objectives
Grading Rubric:
  - Criteria 1: [0-4] points
  - Criteria 2: [0-4] points
  - Criteria 3: [0-4] points
Total Points: 12
```

### Assignment Templates
- Assignment objectives
- Instructions
- Submission format
- Success criteria
- Rubric

## Media Management

### Large Files (Git LFS)
This repository uses Git LFS for:
- Videos (> 100MB)
- High-res images (> 10MB)
- Audio files (> 50MB)
- Datasets (> 100MB)

#### Setting up Git LFS
```bash
git lfs install
git lfs track "*.mp4"
git lfs track "*.pdf"
git add .gitattributes
```

### Copyright & Licensing

All content must include:
- **Copyright holder**: Who owns the content
- **License**: CC-BY, CC-BY-SA, MIT, proprietary, etc.
- **Usage rights**: Can students redistribute? Modify?
- **Attribution requirements**: How to cite

See [docs/LICENSING.md](docs/LICENSING.md) for details.

## Content Submission

### New Course Submission
1. Create course directory following naming conventions
2. Include syllabus and course overview
3. Organize modules with lesson plans
4. Add required resources (books, videos, etc.)
5. Create grading rubrics
6. Submit PR for review

See [docs/SUBMISSION.md](docs/SUBMISSION.md) for:
- Content standards
- File naming conventions
- Metadata requirements
- Accessibility requirements

## Accessing Content

### For Students
- Content available through Moodle LMS
- Synchronized from this catalog
- File versioning controlled by Git

### For Instructors
- Content available for copying to own courses
- Can customize and extend
- Submit improvements back

### For Developers
```bash
# Clone catalog
git clone https://github.com/zsel/zsel-catalog

# Set up Git LFS
git lfs install

# Verify LFS files
git lfs ls-files
```

## Content Organization

See [docs/ORGANIZATION.md](docs/ORGANIZATION.md) for:
- Naming conventions
- Directory structure standards
- File organization
- Metadata templates

## Integration

### With Moodle
- Content automatically imported into Moodle
- Updates synchronized daily
- Version control maintained

### With Student Dashboard
- Course listings from catalog
- Assignment visibility
- Resource access

## Contributing

### Content Contributions
1. Fork the repository
2. Create content in proper directory
3. Follow organization standards
4. Submit PR with metadata
5. Incorporate feedback

### Content Translation
Help translate content to additional languages:
- Create translated_content/[language-code]/ directory
- Use same file structure as English version
- Include translation note in metadata

## License

Content licensing varies:
- **Open Content**: CC-BY-SA (attribution required)
- **Proprietary Content**: Restricted use (ZSEL only)
- **Academic Papers**: Check copyright holder

See [docs/LICENSING.md](docs/LICENSING.md) for complete policy.

---

**Maintainers**: Content Team  
**Last Updated**: March 11, 2026
