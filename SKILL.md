---
name: prompt-improver
description: Turns a short, weak or unclear request into a strong, detailed prompt. Understands any language, including Tamil, Hindi, Telugu and mixed or English-letter writing (Tanglish, Hinglish). Use when the user asks to improve a prompt or gives a rough idea in any language.
---

# Prompt Improver

## Purpose
Many people write short or unclear prompts, and AI gives weak answers.
This skill takes a rough request in ANY language and rewrites it as a
clear, complete prompt that an AI system can follow well.
The user does not need technical knowledge.

## Step 1: Understand the language
- Detect the language the user wrote in.
- Many users write their language in English letters
  (example: "enakku oru post ezhuthu" is Tamil, "mujhe ek email likhna hai"
  is Hindi). Read these by sound and meaning, not by spelling.
- Users often mix languages in one sentence (Tamil + English, Hindi + English).
  Understand the full meaning of the mixed sentence.
- Spelling mistakes and short forms are normal. Guess the meaning
  from context and do not point out the mistakes.
- Focus on the real intention, not only the exact words.

## Step 2: Work out what the user really wants
Find these things in the request:
- Goal: what should the AI produce (post, email, plan, story, code)?
- Audience: who will read or use it?
- Topic and details: names, places, numbers, dates. Keep them exactly.
- Tone: friendly, formal, funny, serious?
- Length and format: short, long, list, table?
If something important is missing, make a sensible assumption and
state it in one line. Ask at most ONE question, and only if the
request cannot be done without the answer.

## Step 3: Write the improved prompt
Use this structure:
- Role: who the AI should act as
- Task: exactly what to do
- Context: background the AI needs
- Steps: how to approach the task
- Format: how the answer should look (length, layout, tone)
- Rules: what to include and what to avoid

Keep it clear and in plain words. Do not make it longer than needed.
Never change the user's facts, names or numbers.

## Step 4: Choose the output language
- Write the improved prompt in ENGLISH by default, because most AI
  systems understand English instructions best.
- Add a line telling the AI which language the FINAL answer must be in,
  matching the user's language (example: "Write the final answer in Tamil").
- If the user asks for the prompt itself in their own language, write it
  in that language, in the proper script.
- Write the short explanation to the user in the user's own language.
- Use the script the user would expect: Tamil script for Tamil,
  Devanagari for Hindi, and so on. If the user typed in English letters,
  you may reply in English letters too, unless they ask otherwise.

## Languages supported
Works with any language. Pay special attention to:
Tamil, Hindi, Telugu, Kannada, Malayalam, Bengali, Marathi, Gujarati,
Punjabi, Urdu, English, Spanish, French, German, Portuguese, Arabic,
Chinese, Japanese, Korean, Russian, Indonesian, Turkish.
Also handle mixed styles: Tanglish (Tamil + English), Hinglish
(Hindi + English), Telugu in English letters, and similar.

## Output format
Give the answer in this order:
1. A one-line note on what you understood (in the user's language).
2. The improved prompt in one block the user can copy.
3. One short line on what you improved.

## Examples

Example 1 (Tanglish)
User: "enakku en bakery ku oru instagram post ezhuthu"
Understood: Write an Instagram post for my bakery.
Improved prompt:
  Role: You are a friendly social media writer for a small bakery.
  Task: Write one Instagram post promoting the bakery.
  Context: Small local bakery. Audience is nearby families.
  Format: 3 to 4 short lines, a warm tone, 5 relevant hashtags.
  Rules: Do not invent prices or offers. Write the final post in Tamil.

Example 2 (Hinglish)
User: "meri dukaan ke liye ek achha sa message likho festival ke liye"
Understood: Write a good festival greeting message for my shop.
Improved prompt:
  Role: You are a polite shop owner's assistant.
  Task: Write a festival greeting message for customers.
  Format: Short, warm, 2 to 3 lines. Add a friendly closing line.
  Rules: Do not mention discounts unless given. Write the final message in Hindi.

Example 3 (Telugu in English letters)
User: "naa business kosam oka plan cheppu"
Understood: Give me a plan for my business.
Action: The request is too general, so ask ONE question:
  "What kind of business is it, and what is the plan for
  (marketing, money, or starting)?" Ask it in Telugu.

## Rules to always follow
- Never judge or correct the user's language or spelling.
- Never leave the improved prompt empty or too short.
- Keep names, numbers and facts exactly as the user gave them.
- Do not add made-up facts.
- Be polite and simple. Avoid technical words.
