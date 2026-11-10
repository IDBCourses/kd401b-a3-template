# GUI-Portfolio-Template

[![W3C HTML Validation](https://github.com/IDBCourses/kd401b-a3-template/actions/workflows/html-validation.yml/badge.svg)](https://github.com/IDBCourses/kd401b-a3-template/actions/workflows/html-validation.yml)
[![Accessibility Check](https://github.com/IDBCourses/kd401b-a3-template/actions/workflows/accessibility.yml/badge.svg)](https://github.com/IDBCourses/kd401b-a3-template/actions/workflows/accessibility.yml)

Template for a portfolio project in the GUIs course.

## Automatic checks

Every time you push to `main`, two checks run automatically on GitHub. Their results are shown by the badges at the top of this page: green means passing, red means something needs fixing.

**Make sure both checks pass before you hand in your portfolio.**

### W3C HTML Validation

Checks every `.html` file in your repository, including pages in subfolders, with the official W3C Nu HTML Checker. It catches things like unclosed or misnested tags, missing required attributes, duplicate `id`s and invalid elements.

### Accessibility Check

Opens every page in a browser and tests it against WCAG 2 level AA using pa11y and the axe engine. It catches things like images without alt text, form fields without labels, low colour contrast and missing page language. Automated tools only find some accessibility problems, so you should still test your site yourself, for example by navigating it with only the keyboard.

## Checking your work with pull requests

The checks also run on pull requests, which lets you find out whether new work passes *before* it reaches `main`.

Why this is useful:

- Your `main` branch always stays in a working, passing state, so the version you hand in is never broken by half-finished changes.
- You can experiment freely on a separate branch without worrying about breaking your site.
- The results show up right on the pull request page, so you can see at a glance whether it's safe to merge.

How to do it:

1. Create a new branch for the change you're working on (for example `about-page`).
2. Commit and push your work to that branch.
3. On GitHub, open a pull request from your branch into `main`.
4. Wait for both checks to finish. They appear at the bottom of the pull request.
5. If a check fails, click **Details** to see what went wrong, fix it on your branch and push again. The checks re-run automatically.
6. When both checks are green, merge the pull request.

You can also run either check by hand: open the **Actions** tab, choose the workflow, and click **Run workflow**.

## Finding out what went wrong

1. Click a red badge above, or open the **Actions** tab of your repository.
2. Click the most recent failed run (marked with a red ✗).
3. Click the job, then expand the step that failed:
   - **Validate every HTML page** for HTML errors
   - **Check every HTML page** for accessibility errors
4. Each error lists the file (or page), the line or element, and a description of the problem.
5. Fix the problems, commit and push again. The checks re-run automatically.

You can also check a single page while you work by pasting its code into the [W3C validator](https://validator.w3.org/#validate_by_input).
