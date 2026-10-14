# Prompt Improver (Claude Skill)

Turn a short, weak prompt into a strong, detailed one. Works in **Tamil, Hindi, Telugu** and many other languages, including words typed in English letters (Tanglish, Hinglish).

You do not need any coding knowledge to use this skill.

## What does it do?

You type a rough idea. The skill understands what you really want and rewrites it as a clear prompt with a role, task, context, steps, format and rules. You can then copy that prompt and use it with any AI.

**Example**

You type:
```
enakku en bakery ku oru instagram post ezhuthu
```

The skill replies with:
- What it understood: "Write an Instagram post for my bakery."
- A complete, improved prompt you can copy
- A short note on what was improved

## Languages

Tamil, Hindi, Telugu, Kannada, Malayalam, Bengali, Marathi, Gujarati, Punjabi, Urdu, English, Spanish, French, German, Portuguese, Arabic, Chinese, Japanese, Korean, Russian, Indonesian, Turkish, and mixed styles like Tanglish and Hinglish.

By default the improved prompt is written in English (most AI systems follow English instructions best) and it tells the AI to write the final answer in your language.

## Repository structure

```
prompt-improver-skill/
├── README.md
├── LICENSE
└── prompt-improver/
    └── SKILL.md      <- the skill itself
```

This skill is only written instructions. It does not use Python or any code.

## How to install

### Claude website or app
1. Download this repository as a ZIP (green **Code** button, then **Download ZIP**), or download `prompt-improver.zip` from the Releases page if available.
2. Make sure the ZIP contains the `prompt-improver` folder with `SKILL.md` inside it.
3. In Claude, open **Settings** and find the section for skills.
4. Upload the ZIP and turn the skill on.

### Claude Code
Copy the `prompt-improver` folder into:
- `~/.claude/skills/` to use it in all projects, or
- `.claude/skills/` inside a project to use it only there.

Example (Mac / Linux), after downloading this repository:

```bash
mkdir -p ~/.claude/skills
cp -r prompt-improver ~/.claude/skills/
```

Example (Windows PowerShell):

```powershell
New-Item -ItemType Directory -Force "$env:USERPROFILE\.claude\skills"
Copy-Item -Recurse prompt-improver "$env:USERPROFILE\.claude\skills\"
```

Then start `claude` and ask it to improve a prompt.

## How to install Claude Code

Claude Code is Anthropic's coding assistant that runs in your terminal. You only need it if you want to use this skill there. It needs a paid Claude plan (Pro, Max, Team or Enterprise). The free plan does not include it.

1. Open a terminal:
   - Mac: open the **Terminal** app
   - Windows: open **PowerShell**
   - Linux: open your terminal
2. Run the install command for your system:

   **Mac, Linux, or WSL**
   ```bash
   curl -fsSL https://claude.ai/install.sh | bash
   ```

   **Windows PowerShell**
   ```powershell
   irm https://claude.ai/install.ps1 | iex
   ```

   **Windows CMD**
   ```
   curl -fsSL https://claude.ai/install.cmd -o install.cmd && install.cmd && del install.cmd
   ```

   You can also install with Homebrew (`brew install --cask claude-code`) or WinGet (`winget install Anthropic.ClaudeCode`).
3. Close and reopen the terminal, then check it worked:
   ```bash
   claude --version
   ```
4. Go to any folder and start it:
   ```bash
   claude
   ```
   Your browser opens so you can log in with your Claude account.
5. If something is wrong, run `claude doctor` to check your setup.

On Windows, installing [Git for Windows](https://git-scm.com/download/win) is recommended.

Official guide: https://code.claude.com/docs/en/setup

## How to use

After installing, just write something like:

- `Improve this prompt: write a post about my bakery`
- `இந்த prompt-ஐ மேம்படுத்து: ...`
- `is prompt ko behtar banao: meri dukaan ke liye message`
- `ee prompt ni improve cheyyi: ...`

## How to edit

Open `prompt-improver/SKILL.md` and change the instructions in plain words. Keep:
- the file name exactly `SKILL.md`
- the folder name the same as the `name:` line at the top of the file
- the `description:` line short, because Claude uses it to decide when to use the skill

Then upload the updated folder to Claude again.

## Contributing

Found a sentence in your language that was misunderstood? Open an issue with the sentence, and add it as an example in `SKILL.md`.

## License

MIT. See the `LICENSE` file.
