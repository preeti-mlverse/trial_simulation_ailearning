# Ada's Nesting Boxes

An interactive game that teaches the difference between **Artificial Intelligence**, **Machine Learning**, **Deep Learning** and **Generative AI** — by showing that they are not four rivals, but four boxes each tucked inside the one before it.

Four illustrated characters host the game and explain themselves in their own words, with animated lip-sync and optional synthesised voices.

| Character | Concept | Why them |
| --- | --- | --- |
| Nana Ada | Artificial Intelligence | The oldest and broadest — the field's 1956 matriarch |
| Professor Sam | Machine Learning | Won't take your rules; wants examples |
| Woolly | Deep Learning | Made of layers — the pun *is* the definition |
| Doodle | Generative AI | Makes things instead of judging them |

## How to play

Open `index.html` in any modern browser, or play the hosted version linked at the top of this repo. There is no build step, no server and no network dependency — the whole game, including the character art, is embedded in that single file.

## The journey

Three levels, unlocked in order, with a traveller that hops along a trail between them:

1. **Beginner — Who's who?** Meet all four characters, then work out who said what.
2. **Intermediate — How machines learn.** Hand-written rules versus learning from examples, plus a layer lab that shows what "deep" actually counts.
3. **Advanced — The tricky ones.** Judging versus making, and the cards that catch everyone out (a hundred-layer X-ray reader is deep learning, not generative AI).

Wrong answers cost nothing — the host character explains the answer and encourages you to carry on. Correct answers get confetti.

## The central mechanic

The answer buttons *are* the nesting diagram. Every answer is a physical click inside a nested box, and the rule is always **"pick the smallest box that still fits."** After a dozen answers the hierarchy is muscle memory rather than a fact you were told.

## Grounding

Definitions, dates and examples are drawn from the Wikipedia articles on [Artificial intelligence](https://en.wikipedia.org/wiki/Artificial_intelligence), [Machine learning](https://en.wikipedia.org/wiki/Machine_learning), [Deep learning](https://en.wikipedia.org/wiki/Deep_learning) and [Generative AI](https://en.wikipedia.org/wiki/Generative_artificial_intelligence). The four-layer face example in the layer lab is the illustration used in the Deep learning article itself.

## Technical notes

- Single self-contained HTML file, no dependencies and no build step.
- Character art is embedded as WebP data URIs; portraits were cut out and, for the lip-sync, the painted mouths were removed so animated ones could be drawn over them.
- Lip-sync is three SVG mouth states per character, cycled while text types in. Voices use the browser's `speechSynthesis` and can be toggled off.
- Light and dark themes, responsive down to mobile, and `prefers-reduced-motion` is respected.
