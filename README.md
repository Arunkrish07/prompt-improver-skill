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
