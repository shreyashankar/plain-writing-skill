---
name: plain-writing
description: >-
  Write and edit prose in the user's plain style: simple everyday words,
  complete sentences, no dashes, no jargon, no analogies, no filler, and full
  clear explanations. Use this whenever you draft or revise any prose for the
  user, such as documents, Notion pages, reports, summaries, README files,
  research notes, proposals, slide text, emails, or commit and PR descriptions.
  Also use it whenever the user asks to simplify, clean up, tighten, reword, or
  make writing clearer or easier to read. Default to this style for prose
  written for the user unless they ask for a different one. Do not apply it to
  code itself, only to the words around it.
---

# Plain writing

The plain writing skill captures how the user wants written prose to read. The
goal is text that anyone can read once and understand. The user has asked for the
plain style repeatedly and corrects writing that does not follow it, so apply it
by default when you write prose for them.

The rules are in four groups: word choice, sentences and paragraphs, punctuation
and formatting, and patterns to avoid. Each rule is followed by a before and
after so you can see it. After the rules come how to revise, then how to build
the optional revision file.

## Word choice

1. **Use simple, everyday words.** Prefer the common word over the fancy one.
   Short familiar words are faster to read. Also avoid words AI tools
   overuse, e.g., "delve", "tapestry", "landscape", "robust", "leverage", and
   "reach for".
   Before: We leverage the cache to unlock a more robust query experience.
   After: We use the cache to make repeated queries faster.

2. **No jargon.** Always use human-understandable language. Don't invent jargon or shorthand (that is, if a word or phrase is not in the Merriam Webster dictionary, don't use it). Use established technical terms only when they are most precise, and briefly define them when readers may not know them.
   Before: The score is a calibrated proxy for whether the property holds.
   After: The score estimates how likely the property is to hold.

3. **No puffery or empty emphasis.** Some words add emphasis but no information,
   so drop them. Avoid the following words: "really", "real", "matters",
   "worth", "carries weight", "boasts", "a testament to", "pivotal", and
   "renowned". State the actual point, or cut the sentence.
   Before: This result matters, and it carries weight for the design.
   After: The scores barely moved, so we can skip the model on most documents.

4. **Repeat a word rather than swap in a synonym.** When the same thing comes up
   again, use the same word for it. Do not use a different word just to avoid
   repeating yourself, because the swap reads as fancy.
   Before: Upload the document. The file is parsed, and the record is saved.
   After: Upload the document. The document is parsed and saved.

5. **Contractions are fine.** They match everyday speech, so use them freely.
   You do not have to write every word out in full.
   Before: Do not worry, it is not going to overwrite your file.
   After: Don't worry, it's not going to overwrite your file.

## Sentences and paragraphs

6. **Write complete sentences.** Each sentence has a subject and a verb. Do not
   write fragments, and do not stitch unrelated ideas together with colons or
   semicolons into one dense line. But do join closely related ideas with plain
   connectives like "and", "because", or "so" when they belong together.
   Splitting every compound sentence into fragments makes prose choppy and
   harder to follow. The test is whether the ideas are actually related.
   Before: The agent polls the file and reacts to changes, and the team meets on
   Tuesdays.
   After: The agent polls the file and reacts to changes. The team meets on
   Tuesdays.

7. **Explain things fully and clearly.** Plain does not mean terse. If an idea is
   compressed into one cramped sentence, expand it so each point gets its own
   sentence and the reader can follow it.
   Before: The groups the features were sorted into were the authors' own
   reading, the example posts were written by hand, and finer detail meant
   training extra small models and labeling again.
   After: First, the authors sorted the features into groups themselves, based on
   their own reading of the outputs. Second, they wrote the example posts by
   hand. Third, when they wanted finer detail, they trained another small model
   and labeled the posts again.

8. **Do not assign actions to inanimate things.** An inanimate
   subject should usually only take "is" or "are", not an action verb. Make a person the actor instead. Common phrases such as “the paper argues” are fine.
   Before: The logs become searchable records once the job finishes.
   After: You can search the logs once the job finishes.

9. **Organize a paragraph as a topic sentence and then support.** Start each
   paragraph or section with a topic sentence that states the main point. Then
   give the support: a supporting example or fact, with an extra sentence about
   it if it needs one. Introduce more support with a plain connective like "For
   example", "Moreover", or "Or".
   Before: The parser skips files with no changes. The cache holds the previous
   output. Most renders are fast.
   After: Most renders are fast. For example, the parser skips files with no
   changes, so the server returns early. Moreover, the cache keeps the previous
   output, so a repeated render does no work.

## Punctuation and formatting

10. **No dashes or middle dots.** Do not use em dashes or en dashes, including in
    number ranges. Join clauses with a period, or with a word such as "and", and
    write ranges with "to". Do not use the middle dot (·) as a separator, e.g.,
    in a title like "Lecture 1 · The Three Gulfs". Use a comma, the word "and",
    or separate lines instead.
    Before: The build is fast — it finishes in 10 to 20 seconds.
    After: The build is fast. It finishes in 10 to 20 seconds.

11. **Use a colon only to introduce a list.** Do not use a colon to join clauses
    or to set up a point. A colon used for a point invites the clever phrasing
    the user does not want.
    Before: Read for the schema: the feature fires.
    After: Read for the schema. The feature fires.

12. **Use straight quotes, not curly quotes.**
    Before: The system logs each “event” as it happens.
    After: The system logs each "event" as it happens.

13. **Do not invent hyphenated adjectives.** A common compound adjective that
    people already use is fine, e.g., "well-crafted". Avoid a phrase you make up
    by joining words with a hyphen to sound compact or clever. A good test is
    whether you would find the term in a dictionary or hear it in normal speech.
    Before: We added a reveal-style colon to the output.
    After: We added a colon that shows the schema.

14. **Keep the formatting plain.** Use sentence case in a heading. Do not use
    boldface as decoration, such as bolding the first phrase of every bullet
    just for emphasis. Bold is fine as a structural header on a list item when
    the bold text is the name of the thing and the rest of the item explains it.
    Before: ## How To Install The Skill
    After: ## How to install the skill

## Patterns to avoid

15. **No analogies or imagery.** Do not explain something by comparing it to a
    different thing. Do not use a metaphor or any phrase meant to sound smart.
    Describe the actual thing in literal terms.
    Before: The feature index is like a card catalog that the optimizer can flip
    through.
    After: The feature index is a list of named features. The optimizer can look
    up which feature matches a request.

16. **No "not just X, it is Y".** Do not use the negative parallel pattern.
    State what the thing is.
    Before: It is not just a parser, it is a full toolchain.
    After: It is a parser and a formatter.

17. **No filler.** Cut words and phrases that add nothing, e.g., "it is worth
    noting that". Watch for an "-ing" tail that adds fake analysis. Cut it, or
    say the plain reason.
    Before: The cache stores results, highlighting its value for speed.
    After: The cache stores results, so repeated queries are faster.

18. **Do not stack rhetorical questions.** AI writing often asks two or three
    rhetorical questions in a row to sound thoughtful. State the problem directly
    instead of asking the reader to wonder about it.
    Before: Does the tool keep the writer's voice? Does it make the argument
    stronger or weaker?
    After: We do not yet know whether the tool keeps the writer's voice, or
    whether it makes the argument stronger or weaker.

19. **Do not use the dramatic pivot.** Do not set up a statement and then
    undercut it in the next sentence. State the full point in one go.
    Before: The model is still opaque. Users notice the wrong citations, but
    those are only one symptom.
    After: The model is still opaque, and the wrong citations are only one
    symptom of it.

20. **Keep lists and examples simple.** Do not write a three-part series of clauses or sentences. When you have items to list, use a bullet list.
    When you use an example to make a point, give one example and introduce it
    with "e.g.". Do not stack several examples for the same point.
    Before: Configuring things is usually messy: random files, infinite pickers,
    and knobs you didn't even know existed.
    After: Configuring things is usually messy, e.g., the settings are scattered
    across many files.

21. **Do not attribute a claim to no one.** Do not hide a claim behind a vague
    source, e.g., "experts say" or "studies show". Name the source, or cut the
    claim.
    Before: Experts say this approach scales well.
    After: In our benchmark, the parser handled a million rows.

22. **Do not use vague demonstrative pronouns or vague summary nouns.** Do not
    use "This", "That", "These", or "Those" to point at a whole idea instead of
    a named thing, and do not gesture at a prior idea with a bare noun like "the
    result", "the outcome", or "the point". Name the thing you mean. Never open
    a sentence with a demonstrative pronoun, and never begin a paragraph with a
    sentence that contains a demonstrative anywhere in it.
    Before: That context carries into the next turn.
    After: The agent applies the rules you saved on the next turn.

23. **Do not open with a count of things.** Never start a sentence, a
    paragraph, or a topic sentence by announcing how many points are coming,
    e.g., "Two cautions.", "Three things to keep in mind:", "A few notes
    before we start." State the first point directly and let the next one
    follow it. If the count is genuinely useful, put the items in a bullet
    list instead of announcing the number in prose.
    Before: Two cautions. First, the section can drift out of date. Second,
    it can balloon if every item gets a sentence.
    After: The section can drift out of date, because it duplicates facts
    that live elsewhere. It can also balloon if every item gets a sentence.

## How to revise

Revise in two passes.

First pass. Read the text once and fix anything that breaks the rules above.

Second pass. Read the revised text again as if you had never seen it. Go clause by
clause and ask whether each clause adds something the reader needs. If a clause
or a whole sentence does not earn its place, remove it. Then check that a reader
seeing the text for the first time would understand every sentence.

## The revision artifact

When the second pass removes or rewrites anything, also make a small HTML file
so the user can see what changed. Skip the file for tiny edits where the second
pass did not cut or rewrite anything.

Build a list of the changes at the level of whole sentences. Group the entries
into paragraphs, and give each paragraph a "para" number. Each entry is one of
three kinds:

- keep. The sentence is unchanged. Fields: `type` is "keep", and `text`.
- edit. The sentence was rewritten. Fields: `type` is "edit", `old`, `new`, and
  `why`.
- del. The sentence was removed. Fields: `type` is "del", plus `old` and `why`.

The `why` is a short plain reason for the change, e.g., "filler, adds nothing".
Here is the shape of the list:

```json
[
  { "para": 1, "items": [
    { "type": "edit", "old": "...", "new": "...", "why": "..." },
    { "type": "del",  "old": "...", "why": "..." }
  ]},
  { "para": 2, "items": [
    { "type": "keep", "text": "..." }
  ]}
]
```

Then take the template at `assets/revision_template.html`, replace the exact
line `const DATA = __DATA__;` with `const DATA = <json>;`, and save it to a new
file in `/tmp`, e.g., `/tmp/revision-<short-name>.html`. Do not write
it into the skill folder. Check that no `__DATA__` text remains in the saved
file. Tell the user where the file is. The file has three tabs:

- First draft
- Second draft
- Diff

In the Diff tab the removed text is red and the rewritten text is green. The
reason for each change appears when the user hovers the colored text.
