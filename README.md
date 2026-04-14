# WaaTech Digital — WordPress Developer Assessment

## 👋 Welcome

This is a take-home coding test for the WordPress Developer position at WaaTech Digital.
You have from **April 13 (Sunday) to April 14 (Monday) 11:59 PM BST** to complete and submit.

---

## 🛠 What You Need (ALL FREE)

- A code editor (VS Code is free — https://code.visualstudio.com/)
- Git installed on your computer (https://git-scm.com/)
- A free GitHub account (https://github.com/)
- A web browser (Chrome recommended for Figma inspect)
- PHP installed locally (for Task 2 and 3 — XAMPP is free: https://www.apachefriends.org/)
- **That's it. Nothing paid. No WordPress. No Elementor. No licenses.**

---

## 📋 How This Works

### Step 1 — Fork this repo
Click the "Fork" button at the top-right of this GitHub page.
This creates your own copy of this repo under your GitHub account.

### Step 2 — Clone your fork to your computer
```bash
git clone https://github.com/YOUR-USERNAME/otwptest.git
cd otwptest
```

### Step 3 — Do the 3 tasks (explained below)

### Step 4 — Commit your work as you go
**IMPORTANT RULE:** You must make **at least 10 commits** while working.
Each commit message must say what you did in that commit.

Good commit examples:
- `"add html structure for hero section"`
- `"style the services cards grid"`
- `"fix mobile responsive breakpoint for doctor section"`
- `"add hover states on buttons"`

Bad commit examples:
- `"update"` (says nothing)
- `"done"` (says nothing)
- `"asdf"` (not a real message)

We check your commit history. We look at timestamps, the changes in each commit, and whether
your work shows a natural progression. This is how we know YOU did the work.

### Step 5 — Push and share
```bash
git push origin main
```
Then send your GitHub repo link to us by **April 14, 11:59 PM BST**.

---

## 📝 The 3 Tasks

### TASK 1 — Build the Homepage (50 points)

**What:** Open the Figma file (link in `reference/FIGMA-LINK.md`). You will see a dental clinic
homepage design with 3 sections (Hero, Our Practice, Doctor). Build these 3 sections using
pure HTML and CSS.

**Rules:**
- Write your code in `task-1-html-css/index.html` and `task-1-html-css/css/style.css`
- The starter files already have Google Fonts loaded and CSS variables set up for you
- Use the Figma inspect panel to get exact colors, spacing, font sizes, paddings
- **Must be responsive at 3 breakpoints:** Desktop (1440px), Tablet (768px), Mobile (320px)
- NO Bootstrap, NO Tailwind, NO CSS frameworks — raw CSS only
- For images, you can use placeholder images from https://placehold.co/ (example: `https://placehold.co/519x540` for a 519×540 image) or export from Figma
- Hover states on buttons are shown in the Figma file — implement them with CSS `:hover`

**What we check:**
- Does it look like the Figma design? (visual accuracy)
- Does it work on all 3 screen sizes? (responsive)
- Is your CSS clean? (no `!important` spam, organized selectors, logical class names)
- Did you use the correct fonts, sizes, colors from Figma?

**How to use Figma Inspect (FREE):**
1. Open the Figma link
2. Click on any element
3. On the right panel, you see: width, height, padding, margin, font-family, font-size, color, etc.
4. You can copy CSS values directly
5. Click on colors to copy hex codes
6. This works on any free Figma account — no paid plan needed

---

### TASK 2 — PHP Template Logic (30 points)

**What:** Open `task-2-php-logic/doctor-template.php`. You will find a PHP array that contains
data for 4 doctors (name, photo URL, specialty, credentials list). Your job is to write PHP
code that loops through this array and outputs proper HTML.

**Rules:**
- Write your PHP code in the same `doctor-template.php` file, below the data array
- Use `foreach` to loop through the doctors
- Use `esc_html()` function (already defined in the file) to escape all output — this prevents XSS
- Each doctor should output: photo, name in an H3, specialty in a paragraph, and credentials as a `<ul>` list
- Check `expected-output.md` to see the expected HTML structure
- You can test by running: `php task-2-php-logic/doctor-template.php` in your terminal

**What we check:**
- Can you write a PHP foreach loop? (basic PHP)
- Do you escape output with esc_html()? (security awareness)
- Does the HTML structure match the expected output? (attention to detail)
- Is the code clean and readable?

---

### TASK 3 — Find and Fix the Bugs (20 points)

**What:** Open `task-3-debug/broken-page.php`. This file has a simple WordPress-style page
with 5 bugs hidden in it. Find all 5 bugs and fix them.

**Rules:**
- Fix the bugs directly in `broken-page.php`
- **Make a separate commit for each bug fix** (5 bugs = 5 commits minimum for this task)
- Each commit message should say what bug you found and how you fixed it
- Read `debug-hints.md` for the categories of bugs to look for

**What we check:**
- Did you find all 5 bugs?
- Did you commit each fix separately with a clear message?
- Do your fixes actually work?

---

## ⏰ Timeline

| When | What |
|------|------|
| April 13 (Sunday) | You receive this repo link. Start anytime. |
| April 13-14 | Work on the tasks at your own pace |
| April 14 (Monday) 11:59 PM BST | **DEADLINE** — your last commit must be before this time |
| April 15 (Tuesday) | We review submissions and score |

---

## ❓ FAQ

**Q: Can I use AI tools like ChatGPT or Copilot?**
A: You can use them as reference, but remember — we check your commit history. If you paste
one giant chunk of code in a single commit, it's obvious. Also, in our office you will need
to do this kind of work daily without AI writing everything. Show us YOUR skill.

**Q: My HTML doesn't look pixel-perfect, is that OK?**
A: We don't expect pixel-perfect. We expect "close to the design with good CSS practices."
If your spacing is off by a few pixels, that's fine. If the layout is completely wrong, that's not fine.

**Q: I don't know how to use Git.**
A: If you're applying for a developer position and don't know Git basics, please learn before
starting. Here's a free 15-minute tutorial: https://guides.github.com/introduction/git-handbook/

**Q: Can I add extra features or animations?**
A: Focus on getting the 3 tasks right first. If you have time and want to add extras, go ahead.
But a clean, accurate, responsive build beats a fancy but broken one every time.

**Q: What if I can't finish everything?**
A: Submit what you have. Partial work is better than no submission. We score each task separately.

---

## 🚀 Good luck!

Show us what you can build. We're looking for developers who:
- Can read a Figma design and turn it into clean code
- Write organized, readable CSS
- Understand basic PHP templating
- Can debug code and explain what they fixed
- Use Git properly with meaningful commits

We look forward to seeing your work! 💪
