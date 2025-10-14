# Resume Modularization Workflow

This repository uses a modular LaTeX structure for easy creation of multiple resume versions.

## Quick Links

- [One-Page Resume](build/main_onepage.pdf)
- [Full Resume](build/main_full.pdf)

## Structure

- `sections/education.tex` — Education section
- `sections/experience.tex` — Experience section
- `sections/projects.tex` — Projects section (customize for each application)
- `sections/skills.tex` — Technical skills
- `sections/highschool.tex` — Further highschool experience
- `main_full.tex` — Full resume (all sections)
- `main_onepage.tex` — One-page resume (key sections only)

## Creating Custom One-Page Resumes

1. **Duplicate `main_onepage.tex`** for each application (e.g., `main_onepage_data.tex`, `main_onepage_webdev.tex`).
2. **Customize included sections** by editing which `\input{}` files are included.
3. **Create alternate section files** (e.g., `projects_data.tex`, `projects_webdev.tex`) for tailored content.
4. **Edit the main file** to include the relevant section files for each job.

## Example
```latex
% main_onepage_data.tex
\input{sections/education}
\input{sections/experience}
\input{sections/projects_data}
\input{sections/skills}
```