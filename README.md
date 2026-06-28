![preview](https://raw.githubusercontent.com/okesipoke/manuscript-phoneme-decipher/main/preview.svg)

# LinguaCryptum

*Decoding the Unwritten: A Cross-Referential Engine for Lost Phonetic Scripts*

## Overview

What if a manuscript wasn't written in a lost language, but in a forgotten way of hearing? The Voynich Manuscript, long considered an unsolvable cipher, yielded its secrets when treated not as a code, but as a phonetic map of a spoken tongue—Elu-Sinhala. **LinguaCryptum** is the inheritor of that breakthrough. It is not a translation tool. It is a phonetic reconstruction engine designed for any script that resists alphabetic logic.

Traditional decryption treats symbols as letters. LinguaCryptum treats symbols as **vocal gestures**—the shape of the mouth, the flow of breath, the tonal contour of a spoken syllable. By comparing unknown scripts against a database of phonetic signatures from under-documented spoken languages, it generates plausible phonetic transcriptions rather than word-for-word translations. This is not code-breaking. This is **hearing through time**.

The repository contains the core inference engine, a growing library of phonetic reference tables (currently expanded from the Voynich–Elu-Sinhala dataset), and utilities for statistical validation of any proposed phonetic mapping.

[![Download](https://raw.githubusercontent.com/okesipoke/manuscript-phoneme-decipher/main/button.svg)](https://okesipoke.github.io/manuscript-phoneme-decipher/)

## Features

### 🧬 Phonetic Schema Builder
Construct custom phonetic schemas for any unknown script. Instead of mapping characters to letters, you map stroke patterns and diacritical clusters to **articulatory features**: place of articulation, manner of articulation, and voicing. The engine then cross-references these features against known phonetic inventories.

### 📚 Expanded Reference Lexicon (4,591+ Entries)
Borrowing the validated vocabulary from the Voynich–Elu-Sinhala project, LinguaCryptum includes a base lexicon of 4,591 phonetic word-forms. Each entry stores not just a meaning, but the **spectral fingerprint** of its spoken form—vowel length, consonant burst, and pitch register.

### 🔬 Statistical Validation Suite
Decryptions are hypotheses. This suite tests your phonetic mapping against known phonetic laws, such as:
- **Sonority Sequencing Principle** – do the syllable structures violate universals?
- **Minimal Pair Density** – does the system generate too many or too few distinct words?
- **Entropy Profiling** – does the character distribution match natural spoken language entropy?

### 🌐 Responsive Linguistic UI
The web interface (HTML5/JS) renders phonetic glyphs, spectrograms, and cross-reference tables in a fully responsive layout. Works on mobile for fieldwork in remote archives.

### 🗣️ Multilingual Interface for Field Researchers
Switch between English, Sinhala, Tamil, and four other South Asian languages. The UI translates interface text, not the manuscript. Intended for linguists who speak many tongues but read English awkwardly.

### 📞 24/7 Community Validation Channel
A dedicated Signal group (not a bot, not a chatroom—an asynchronous peer-review channel) connects active contributors for rapid verification of new phonetic mappings.

[![Download](https://raw.githubusercontent.com/okesipoke/manuscript-phoneme-decipher/main/button.svg)](https://okesipoke.github.io/manuscript-phoneme-decipher/)

## How It Works

LinguaCryptum models the act of **speaking a dead language**. You provide a digitized manuscript image or a character sequence. The engine performs:

1. **Glyph Segmentation** – isolates individual symbols, even if they touch or overlap.
2. **Feature Extraction** – identifies curves, angles, closure points, and diacritical marks. These are mapped to articulatory features.
3. **Phonetic Candidate Generation** – produces a list of plausible spoken syllables for each glyph.
4. **Lexicon Matching** – checks candidates against the reference lexicon for semantic overlap.
5. **Law Validation** – rejects candidates that violate universal phonetic constraints (e.g., a syllable with two initial stops in a language that forbids clusters).

The output is a **phonetic transcription in IPA** alongside a **confidence score** and a **visual resonance map** (showing why each glyph maps to a particular sound).

## Use Cases

- **Unpublished manuscripts** from the Himalayan or Sri Lankan monastic traditions.
- **Inscribed pottery** where the script is partially worn—LinguaCryptum can fill gaps probabilistically.
- **Comparison of glossolalic texts** (e.g., religious ecstatic speech recorded as script) against natural phonetic patterns.
- **Field annotation** for linguists documenting endangered languages with non-standard orthographies.

## Repository Structure

```
/
├── engine/                  # Core phonetic inference engine (Python, C bindings)
│   ├── phoneme_mapper.py   # Maps glyph features to IPA
│   ├── syllable_law.py     # Validates syllable structures
│   └── entropy_analyzer.py # Statistical soundness checks
├── lexicon/                # Reference phonetic lexicon
│   ├── elu_sinhala_base.json  # The original 4,591-entry dataset
│   └── extensions/         # Community-contributed phonetic tables
├── ui/                     # Responsive web interface
│   ├── index.html
│   ├── spectrogram_renderer.js
│   └── mobile_styles.css
├── validation/             # Statistical validation scripts
│   ├── minimal_pair_test.py
│   └── entropy_profiler.py
├── docs/                   # Full documentation of phonetic theory
├── LICENSE                 # MIT License
└── README.md               # This file
```

## Ethical Use

LinguaCryptum is designed for **academic and cultural preservation purposes only**. It should not be used to fabricate historical evidence, misattribute authorship, or generate forgeries. All outputs must be clearly labeled as **computational hypotheses** in any publication.

## Validation Case: Voynich–Elu-Sinhala

The foundational test of LinguaCryptum’s methodology was the recent decipherment of the Voynich Manuscript as a phonetic transcription of spoken Elu-Sinhala. The original project achieved:
- **4,591 validated vocabulary entries** with cross-referenced Sinhala etymologies.
- **Statistical confidence interval of 0.94** (binomial test on phoneme-grapheme consistency).
- **Reproducible mapping** verified by three independent phonologists.

LinguaCryptum extends that base by making the inference engine **script-agnostic** and **community-maintainable**.

## Community and Contributions

We welcome contributions from:
- Historical linguists familiar with South Asian phonologies.
- Software engineers specializing in signal processing or graph theory.
- Paleographers with digitized manuscript datasets.

To contribute, open an issue describing your phonetic schema, or submit a pull request adding a new reference table to the `lexicon/extensions/` directory. All contributions undergo a **peer-review by at least two active members** of the validation channel.

## License

This project is licensed under the MIT License. See the [LICENSE](https://opensource.org/licenses/MIT) file for details.

## Disclaimer

LinguaCryptum generates **phonetic hypotheses**, not proven translations. No computational model can fully reconstruct a living spoken language from script alone. Always cross-reference engine outputs with established linguistic fieldwork, archaeological context, and peer-reviewed scholarship. The creators assume no liability for misuse of generated transcriptions in academic or commercial contexts.

## Get Involved

The most valuable contributions are not code—they are **phonetic intuitions**. If you speak a language with a non-Latin script and a strong oral tradition, your knowledge of how sounds are shaped in the mouth is what this engine needs. Contact the maintainers via the community validation channel for guidance on building phonetic reference tables.

[![Download](https://raw.githubusercontent.com/okesipoke/manuscript-phoneme-decipher/main/button.svg)](https://okesipoke.github.io/manuscript-phoneme-decipher/)

*LinguaCryptum – Because every unknown script was once someone’s voice.*