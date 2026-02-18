Your job is to rate how well the text is normalized. Normalized text is written the way it was spoken; some elements might need to be spelled out. Normalized text should follow certain rules:

- All numerals converted into words (**1.5** → one point five)
- Special characters replaced with word equivalents (**%** → percent)
- Initialisms (initial letters pronounced separately) separated into letters (**FBI** → F B I)
- Acronyms that are pronounced as a word should remain unchanged (**NASA** → NASA)
- Numeral abbreviations converted into words (**90s** → nineties)
- Common abbreviations expanded into full words (**etc.** → et cetera)
- Dates expanded into full words (**1.01.2025** → first of January of twenty twenty five OR January first twenty twenty five)
- Contractions like "I'm" and "we'd" stay as they are
- No punctuation is retained, except the dot at the end of a sentence

---

There are two types of normalization errors:

- **Level 1 error** – The model identified a part that needed normalization but failed to follow the rules correctly.
- **Level 2 error** – The model failed to identify a part of the sentence that required normalization.

---

## Scoring

- **5** is for text where all elements are normalized exactly according to the rules.
- **4** is for text that has one Level **1** error.
- **3** is for text that has two Level **1** errors, or one Level **2** error.
- **2** is for text that has three Level **1** errors, or a combination of one Level **2** and one Level **1** error.
- **1** is for text that has more than three Level **1** errors, or more than one Level **2** error.

> **Please note** that any other issues (grammar or style issues in original sentences) are not to be taken into consideration. We are only interested in assessing the quality of the normalization step.