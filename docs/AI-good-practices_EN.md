# GOOD PRACTICES WITH AI

<p align="center"><i>"AI isn't intelligent, it's cultured."</i></p>

A short guide to get more out of AI in everyday use. AI answers aren't always correct: it can make mistakes even when it has the right information.

## Prompt structure

Persona *(optional)* → **Context** → **Task** → **Format**

> [!TIP]
> AI itself can write your prompts for you!

**Example:** You are a customer service expert *(←Persona)*. Our company has accumulated serious order delays due to a courier issue and several customers have complained *(←Context)*. Write an apology message to calm them down *(←Task)* presented as a template with blanks to fill in *(←Format)*.

> [!NOTE]
> The first prompt rarely gives the desired result on the first try; you need to continue the conversation asking for adjustments until you get there.

> [!NOTE]
> Attaching examples significantly improves prompts.

## Heavy lifting

<p align="center"><i>"Don't let AI do the work, use it to build the tools that will."</i></p>

### Wrong

**Example:** "Remove the duplicates and sort this list of emails alphabetically: ..."

**Result:** Omitted information, hallucinations, inaccuracy, degraded attention, truncated responses, etc.

### Correct

**Example:** "Write a Python program to remove duplicates and sort this list of emails alphabetically: ..."

**Result:** A correctly structured list with all the data intact. Plus, you can reuse the same procedure on a new list (as long as it keeps the same format, of course).

<p align="center">THE PROGRAM DOESN'T READ THE INFORMATION, IT PROCESSES IT.</p>

## Changes in large files

You can't expect AI to generate an entire 2,000-line file, error-free, all at once through the chat.

If the changes are small, **ask only for the modified lines**.

If there are many changes, there are **two options**:
* **Ask for the updated file to download:** Request that it offer a download button with the finished document ready (not all AIs allow this).
* **Work locally:** Consider using AI directly from the desktop (instead of the web version) so you can edit files directly on your hard drive.

## Session rules

As the conversation grows, the context window fills up and the quality of the responses degrades. That's why it's a good idea to start fresh often:

* **Task finished**: Start a **new session**.
* **AI is hallucinating**: Run a **"handoff" prompt** → Start a **new session** *(with a summary + the required files)*.

> [!NOTE]
> A **"handoff" prompt** is an instruction you ask AI for before closing the session so it summarizes the state of the work (what's been done, what's left, and which files are needed), so you can paste that summary into the new session and continue without losing context.

## Glossary

* **Prompt**: the instruction or text you write to the AI.
* **Context window**: everything the AI "remembers" within the same conversation. It has a limit, and once it fills up, response quality drops.
* **Token**: the unit in which AI measures text. The actual calculation is complex, but as a simple rule: about 3 words equal roughly 4 tokens (depending on the language).
