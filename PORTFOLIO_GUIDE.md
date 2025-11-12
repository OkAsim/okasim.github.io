# Asim's Portfolio - User Guide

This guide will help you maintain and update your portfolio website.

## Website Structure

Your portfolio is built with Jekyll using the Chirpy theme and hosted on GitHub Pages at `https://okasim.github.io/`

### Main Files & Folders:

```
okasim.github.io/
├── _config.yml          # Site configuration (title, description, etc.)
├── _tabs/               # Main navigation pages
│   ├── about.md         # About page
│   ├── projects.md      # Projects portfolio
│   ├── research.md      # Research & Notes
│   ├── archives.md      # Blog archives
│   ├── categories.md    # Blog categories
│   └── tags.md          # Blog tags
├── _posts/              # Blog posts (YYYY-MM-DD-title.md format)
├── assets/              # Images, CSS, JavaScript
├── robots.txt           # Prevents search engine indexing
└── PORTFOLIO_GUIDE.md   # This file
```

---

## Privacy Settings

**Important:** Your website has `robots.txt` configured to discourage search engines from indexing it. This means:

✅ People with the direct link can access it
✅ You can share it with professors and programs
❌ It won't show up easily in Google searches

If you want to change this, edit or delete the `robots.txt` file.

---

## How to Update Content

### 1. Update Your About Page

Edit `_tabs/about.md` to:
- Add new achievements
- Update current coursework
- Add new books you've read
- Update your goals

### 2. Add New Projects

Edit `_tabs/projects.md` to:
- Add completed Python projects with code examples
- Update Qiskit progress with circuits you've built
- Add documentation or videos from the hoverboard project
- Include GitHub repositories for your projects

### 3. Add Research Notes

Edit `_tabs/research.md` to:
- Upload Cornell notes (place PDFs in `assets/notes/`)
- Add summaries of new books
- Document coursework progress
- Share study strategies

### 4. Write Blog Posts

1. Create a new file in `_posts/` folder
2. Name it: `YYYY-MM-DD-title-of-post.md` (e.g., `2025-11-15-learning-qiskit.md`)
3. Use the template in `_posts/YYYY-MM-DD-template-for-new-posts.md`
4. Update front matter (title, date, categories, tags)
5. Write your content in Markdown

**Example front matter:**
```yaml
---
title: My First Quantum Circuit in Qiskit
date: 2025-11-15 14:30:00 -0800
categories: [Quantum Computing, Projects]
tags: [qiskit, quantum-circuits, python, tutorial]
---
```

---

## Adding Images

1. Save images to `assets/img/` folder
2. Reference in your Markdown:

```markdown
![Description of image](/assets/img/filename.jpg)
```

---

## Adding Files (PDFs, etc.)

1. Create a folder: `assets/files/` or `assets/notes/`
2. Add your files there
3. Link to them:

```markdown
[Download Cornell Notes - Chapter 1](/assets/notes/feynman-ch1.pdf)
```

---

## Publishing Updates

After making changes:

```bash
git add .
git commit -m "Description of changes"
git push origin main
```

GitHub Pages will automatically rebuild your site (takes 2-5 minutes).

---

## Markdown Syntax Quick Reference

### Headings
```markdown
# Heading 1
## Heading 2
### Heading 3
```

### Text Formatting
```markdown
**Bold text**
*Italic text*
`Code text`
```

### Lists
```markdown
- Bullet point 1
- Bullet point 2

1. Numbered item 1
2. Numbered item 2
```

### Links
```markdown
[Link text](https://url.com)
```

### Code Blocks
````markdown
```python
def hello():
    print("Hello, World!")
```
````

### Math (LaTeX)
```markdown
Inline: $E = mc^2$

Block:
$$
\psi(x) = A e^{ikx}
$$
```

---

## Customization

### Change Site Title or Tagline
Edit `_config.yml`:
```yaml
title: Asim Ahmed
tagline: Your new tagline here
```

### Change Theme Mode
Edit `_config.yml`:
```yaml
theme_mode: dark  # or light, or leave empty for auto
```

### Add Profile Picture
1. Add image to `assets/img/avatar.jpg`
2. Edit `_config.yml`:
```yaml
avatar: /assets/img/avatar.jpg
```

---

## Tips for Academic Portfolio

### What to Include:
✅ Specific projects with code/documentation
✅ Detailed descriptions of what you learned
✅ Clear goals and research interests
✅ Evidence of sustained effort over time
✅ Cornell notes and study materials
✅ Thoughtful reflections on learning

### What to Avoid:
❌ Vague descriptions without details
❌ Claims without supporting evidence
❌ Overly informal language in main pages
❌ Personal information (specific school names, addresses)

### When Sharing with Professors:
1. Make sure content is up-to-date
2. Include recent projects or notes
3. Add a specific note in your email about what you'd like them to see
4. Check all links work

---

## Troubleshooting

**Site not updating after push?**
- Wait 5 minutes for GitHub Pages to rebuild
- Check the "Actions" tab in your GitHub repository for build status

**Images not showing?**
- Make sure path starts with `/assets/`
- Check file name spelling exactly matches

**Post not appearing?**
- Check filename format: `YYYY-MM-DD-title.md`
- Make sure date in front matter isn't in the future
- Verify front matter syntax is correct

---

## Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Chirpy Theme Wiki](https://github.com/cotes2020/jekyll-theme-chirpy/wiki)
- [Markdown Guide](https://www.markdownguide.org/)
- [GitHub Pages Docs](https://docs.github.com/en/pages)

---

## Need Help?

If you run into issues:
1. Check the Jekyll build log in GitHub Actions
2. Review the Chirpy theme documentation
3. Make sure all YAML front matter is correctly formatted
4. Verify file paths are correct

---

*Good luck with your portfolio! Keep updating it as you learn and grow!*
