# Resume Templates

This folder contains 10 resume templates (5 LaTeX + 5 JSON Resume) that auto-compile to PDF on every push.

## Templates Included

### LaTeX Templates
1. sb2nov
2. Awesome-CV
3. Deedy-Resume
4. ModernCV
5. AltaCV
6. Rover
7. Expressive-Resume

### JSON Resume Themes
1. Elegant
2. Class
3. Stackoverflow
4. Flat
5. Actual

## Structure

```
resume/
├── latex/
│   ├── sb2nov/
│   ├── awesome-cv/
│   ├── deedy-resume/
│   ├── moderncv/
│   ├── altacv/
│   └── rover/
└── json-resume/
    ├── resume.json (single data file)
    └── package.json
```

## How It Works

1. Edit resume content in respective template files
2. Push to `main` branch
3. GitHub Actions automatically compiles all templates to PDF
4. PDFs available as artifacts and in releases

## Local Development

### LaTeX Templates
```bash
cd resume/latex/<template-name>
pdflatex resume.tex
```

### JSON Resume
```bash
cd resume/json-resume
# Edit resume.json
resume export resume-elegant.pdf --theme elegant
```

## Viewing PDFs

Latest compiled PDFs available in GitHub Actions artifacts or releases.
