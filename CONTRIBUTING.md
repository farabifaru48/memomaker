# Contributing to Memo Maker

Thank you for wanting to help. Every kind of help counts, and you do not need to be an expert.
সাহায্য করতে চাওয়ার জন্য ধন্যবাদ। ছোট বড় সব ধরনের সাহায্যই কাজে লাগে।

## Ways to help

- **Report a bug:** open an [issue](https://github.com/USERNAME/memo-maker/issues) and use the Bug report template.
- **Suggest an idea:** open an issue and describe the problem you want solved, not only the solution.
- **Fix a typo or improve a translation:** the Bangla and English texts are in one place (see below).
- **Change the code:** see below.

## Project layout

The whole app is one file: `index.html`. There is no build step and nothing to install.

| Part | Where in `index.html` |
|---|---|
| Styles | the `<style>` block at the top |
| Icons | the `<svg>` block with `<symbol id="i-...">` |
| Page layout (header, chips, form) | the HTML between `<body>` and the pop-up `<div class="sheet">` blocks |
| Pop-ups (business details, business list, memo no. and date, past memos) | the `<div class="sheet" id="...">` blocks, just before the `<script>` tags |
| All Bangla and English texts | the `T` object, with `bn` and `en` inside |
| Memo preview | the `paint()` function |
| PDF | the `getPDF()` function |
| Businesses, default business | `renderBiz()`, `openBiz()`, `addBiz()`, `delBiz()` and the start-up block at the bottom |
| Past memos | `saveMemo()`, `renderHist()` and `openMemo()` |
| Saved data | `localStorage` keys `memo-tool-v2` (businesses and settings) and `memo-tool-v2-history` (past memos) |

## Making a change

### Easiest: in the GitHub web editor

1. Open `index.html` in this repository.
2. Tap the pencil icon (Edit).
3. Make your change. Use your browser's search to find the text you want.
4. Tap **Commit changes**, choose **Create a new branch** and tap **Propose changes**.
5. Tap **Create pull request**, and describe what you changed and why.

### With a copy on your computer

1. **Fork** this repository (button at the top right).
2. Clone your fork, or download `index.html`.
3. Edit it and open it in a browser to test. Double-clicking the file is enough.
4. Commit to a new branch and open a **pull request** to this repository.

## Guidelines

- **Keep it one file and dependency free.** Please do not add a build tool or a framework. Small libraries loaded from a CDN need a good reason and a pinned version.
- **Every visible text needs both languages.** Add the key to both `T.bn` and `T.en`, and use `data-t="key"` in HTML or `t('key')` in JavaScript.
- **Do not change the storage keys or the shape of saved data** without a migration. Users would lose their memos.
- **Escape user input** with `esc()` before putting it into HTML.
- **Keep it small-screen friendly.** Most users are on phones.
- **Keep the PDF working.** The memo preview is what becomes the PDF, so test both.
- Do not copy code or images you do not have the right to use.

## Test checklist

Before you open a pull request, try these in Chrome (phone size if possible). Use a private window to test the first-time setup:

- [ ] First open asks for the business details, and saving them works
- [ ] Switch between Bangla and English
- [ ] Add, edit and delete items, and check the totals
- [ ] Add a logo, a note and a closing message, and check they appear on the memo
- [ ] Switch between Classic and Card designs
- [ ] The memo number and date at the top are filled in, and can be changed
- [ ] Download a PDF, and open it
- [ ] Tap **New memo**. The number goes up by one
- [ ] Find the memo again in **Past memos** and open it
- [ ] Add a second business, make it the default with the star, reload the page and check it opens first
- [ ] Reload the page. Your business details are still there
- [ ] Nothing looks broken on a narrow (phone) screen

## Pull request tips

- One pull request, one topic.
- Say what you changed and why, in a few sentences. Screenshots help.
- Be patient and kind. This is a small project maintained in spare time.

## Code of conduct

Be respectful. No harassment, insults or discrimination. Everyone is here to learn and help.
