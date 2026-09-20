# LLM Co-Author Addresses

A verified list of `Co-authored-by` Git commit trailers for AI coding assistants. 

Use these in your commit messages to give credit to LLMs and have their avatars/identities properly displayed in GitHub commit histories.

##  But why?

You might wonder why would we need this when the AI coding agent already add their own `Co-authored-by` trailer to the commit message. 

The problem is, they don't always do. In fact, Claude Code is probably the only one automatically doing it by default. in Codex, you need to turn on the feature first. In Antigravity CLI, the option doesn't even exist.

You might also want to attribute AI in commits where you use their web interface instead of their AI coding agent, such as Google AI Studio.

---

## 📋 Quick Reference

| Assistant | Commit Trailer | Profile Linked | Contributor |
| :--- | :--- | :---: | :---: |
| **Claude** | `Co-authored-by: Claude <noreply@anthropic.com>` | ✅ | ✅ |
| **Codex** | `Co-authored-by: Codex <noreply@openai.com>` |✅| ✅|
| **Gemini** | `Co-authored-by: gemini-code-assist[bot] <176961590+gemini-code-assist[bot]@users.noreply.github.com>` | ✅ | ✅ |
| **CodeRabbit** | `Co-authored-by: coderabbitai[bot] <136622811+coderabbitai[bot]@users.noreply.github.com>` | ✅ | ✅ |
| **Qwen Coder** | `Co-authored-by: Qwen-Coder <qwen-coder@alibabacloud.com>` |✅|✅|
| **Z.ai (GLM)** | `Co-authored-by: GLM-5.3 <noreply@z.ai>` |✅|❓|

---

## 🛠 How to Use

Git trailers **must be at the very end** of the commit message, separated from the body/subject by a **blank line**.

### Example:

```bash
git commit -m "Refactor auth middleware to support JWT" -m "Co-authored-by: Claude <noreply@anthropic.com>"
```

Or when writing commit messages in an editor:

```txt
Refactor auth middleware to support JWT

Added token refresh logic and improved expiry error handling.

Co-authored-by: Claude <noreply@anthropic.com>
Co-authored-by: Codex <noreply@openai.com>
```

---

## Verification

This repository tests and validates whether GitHub:
1. Resolves the email to a registered GitHub user or GitHub App bot.
2. Shows the AI assistant's avatar in the commit badge.
3. Shows the AI assistant as one of the contributors in the repository's.

## Contributing

Know an official address for another AI assistant (e.g., GitHub Copilot, Cursor, Tabnine)? Feel free to open a PR!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.