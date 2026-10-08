# Contributing to Thesis Desk 🎓

First of all, **thank you** for taking the time to contribute! 🎉
Every contribution — code, documentation, translations, bug reports, or ideas — is appreciated.

> **بالعربية:** شكراً لاهتمامك بالمساهمة في «مكتب الرسالة». كل مساهمة (كود، توثيق، ترجمة، بلاغ خطأ، أو فكرة) مرحّب بها. هذا الملف باللغة الإنجليزية ليصل إلى أكبر عدد من المطوّرين، ويمكنك كتابة قضاياك وطلبات الدمج بالعربية أيضاً بلا مشكلة.

---

## 📜 Code of Conduct

By participating, you agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md).
Please report unacceptable behaviour to **ahmed.a.moharam@outlook.com**.

---

## 💡 Ways to contribute

- 🐛 **Report a bug** — open a [Bug report](../../issues/new?template=bug_report.yml).
- ✨ **Suggest a feature** — open a [Feature request](../../issues/new?template=feature_request.yml).
- 📖 **Improve documentation** — the user guide, README, or comments.
- 🌍 **Translate** — the UI or the guide to other languages (see `README.en.md`).
- 💻 **Write code** — look for issues labelled [`good first issue`](../../labels/good%20first%20issue) or [`help wanted`](../../labels/help%20wanted).
- ⭐ **Star the project** — it helps others discover it.

---

## 🛠️ Tech stack & philosophy

Thesis Desk is intentionally **simple and dependency-free**:

- **Vanilla JavaScript** (no frameworks, no build step, no bundler).
- **HTML5 + CSS3**, RTL-first Arabic design, automatic day/night mode.
- Works fully **offline**; data is stored in the browser via `localStorage`
  (keys `thesis-desk-v2` and `td-api`).
- Optional network calls only to public academic APIs (OpenAlex, Crossref).

**Please keep it that way.** Avoid adding runtime dependencies unless there is a very strong reason. A pull request that introduces a framework or a build system will need a discussion first.

---

## 🚀 Getting started

1. **Fork** the repository and **clone** your fork:
   ```bash
   git clone https://github.com/<your-username>/DBA-Research-Dissertation-Assistant.git
   cd DBA-Research-Dissertation-Assistant
   ```
2. **Create a branch** with a descriptive name:
   ```bash
   git checkout -b feat/bibtex-export
   ```
3. **Run it locally** — no build needed:
   ```bash
   # Option A: open the developer build
   #   just open index.html in your browser
   # Option B: serve it
   python -m http.server 8080
   # then open http://localhost:8080
   ```
4. **Make your changes**, test them in a browser, and commit.
5. **Push** and open a **Pull Request**.

---

## 🗂️ Project structure

```
DBA-Research-Dissertation-Assistant/
├── index.html                  # Main page (developer build)
├── assets/
│   ├── css/style.css           # All styles (day/night)
│   ├── js/app.js               # All application logic
│   └── img/logo.svg            # Logo & icon
├── standalone/
│   └── thesis-desk-v3.html     # Self-contained single file
├── docs/
│   └── guide.html              # Full user guide
└── screenshots/                # Screenshots
```

> ⚠️ `standalone/thesis-desk-v3.html` is a **generated** file. If your change
> affects the app, please regenerate it (inline the CSS/JS/logo) so both builds
> stay in sync, and mention it in your PR.

---

## ✅ Coding guidelines

- Match the existing style; keep functions small and commented.
- Write user-facing text in **Arabic**, and keep it RTL-friendly.
- Never break `localStorage` backwards compatibility without a migration.
- Test in **Chrome, Edge and Firefox** (desktop and mobile widths).
- Check the browser console — pull requests with console errors will be asked to fix them.

---

## 📝 Commit messages

Use clear, conventional prefixes when possible:

```
feat: add BibTeX export for references
fix: prevent duplicate studies in auto generator
docs: clarify APA 7 formatting rules
style: improve dark-mode contrast
refactor: split reference verification helper
```

---

## 🔀 Pull request process

1. Fill in the pull request template.
2. Link the issue it fixes (e.g. `Closes #12`).
3. Make sure the **CI** check passes.
4. Keep pull requests focused — one topic per PR.
5. A maintainer will review as soon as possible. Please be patient and kind. 🙂

---

## 💬 Questions & discussions

Use [GitHub Discussions](../../discussions) for questions, ideas and show-and-tell.

---

## 📄 License

By contributing, you agree that your contributions are licensed under the
[MIT License](LICENSE).