# 📰 Year 7 English — The Student Press

Interactive grammar lessons built around the theme of news reporting, designed for Year 7 students. Each lesson is a standalone HTML file that runs directly in the browser — no installation or build step needed.

**Live site:** [View on GitHub Pages](https://yourusername.github.io/your-repo-name/)

---

## 📚 Lessons

### Vol. I — Mastering Passive Voice
`passive-voice.html`

A 6-slide interactive lesson teaching students how and why journalists use passive voice.

- Active vs Passive voice comparison
- The journalist's reasons for using passive voice
- Tense and structure rules
- Multiple-choice practice questions
- Headline Builder activity
- Open writing challenge

---

### Vol. II — Direct & Indirect Speech
`direct-indirect-speech.html`

An 8-slide interactive lesson on quoting sources in news articles, with AI-powered feedback.

- Introduction with direct vs indirect speech comparison
- Grammar rules: tense backshift table, pronoun changes, time expressions
- When to use each type (journalist's style guide)
- Multiple-choice quiz (3 questions)
- Quote Builder activity (indirect speech sentence construction)
- Writing challenge: Direct → Indirect speech (AI feedback)
- Writing challenge: Indirect → Direct speech (AI feedback)
- Reporting verbs word bank with 4-question interactive game

---

## 🚀 Running Locally

No server or build tools required. Just open any HTML file directly in your browser:

```
index.html                   ← Landing page (links to both lessons)
passive-voice.html           ← Lesson 1
direct-indirect-speech.html  ← Lesson 2
```

Or double-click any `.html` file in your file explorer.

---

## 🌐 Deploying to GitHub Pages

1. Push this repository to GitHub
2. Go to **Settings → Pages**
3. Under **Source**, select **Deploy from a branch**
4. Choose `main` branch and `/ (root)` folder
5. Click **Save**

Your site will be live at:
```
https://yourusername.github.io/your-repo-name/
```

> Replace `yourusername` and `your-repo-name` with your actual GitHub username and repository name.

---

## 🤖 AI-Powered Feedback

The Direct & Indirect Speech lesson uses the **Anthropic Claude API** to give students personalised feedback on their written answers.

The API is called client-side from the browser. For this to work on GitHub Pages, the Claude.ai interface must be used (which handles API authentication automatically). If you are hosting this independently and wish to enable the AI feedback feature, you will need to add your own Anthropic API key.

To add your own API key, locate the `fetch` calls in the `<script>` section of `direct-indirect-speech.html` and add an `x-api-key` header:

```js
headers: {
  "Content-Type": "application/json",
  "x-api-key": "YOUR_API_KEY_HERE",
  "anthropic-version": "2023-06-01"
}
```

> ⚠️ Never commit a real API key to a public repository.

---

## 🗂 File Structure

```
/
├── index.html                    ← Landing page
├── passive-voice.html            ← Vol. I lesson
├── direct-indirect-speech.html   ← Vol. II lesson
└── README.md                     ← This file
```

---

## ✏️ Customisation

All lessons are single self-contained HTML files with inline CSS and JavaScript — no external dependencies except Google Fonts and the Anthropic API.

To edit content:
- Open the HTML file in any text editor
- Slides are clearly marked with comments like `<!-- ══════════ SLIDE 1 ══════════ -->`
- Quiz questions, writing prompts, and feedback text are all editable directly in the HTML

---

## 📄 Licence

Created for classroom use. Free to adapt and share for educational purposes.
