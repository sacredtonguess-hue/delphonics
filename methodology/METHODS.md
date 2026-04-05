# Delphonics Methodology (v1.0)

## I. Structural Hierarchy (The Triple-Layer Logic)
To reconstruct the source audio, apply the following linguistic priority to every string:

1. **Primary (Sanskrit/Vedic):** The **Morphological Skeleton**. Defines case endings, dual/plural suffixes, and core noun roots (e.g., *janane*, *kāye*).
2. **Secondary (Prakrit):** **Phonetic Shifts**. Accounts for vowel assimilation and consonant softening (e.g., *j* to *y* shifts) found in the oral delivery.
3. **Tertiary (Marathi):** **Kinetic/Intensive Phrasing**. Provides percussive or colloquial vocabulary and governs "final suffix dropping" (e.g., *koṇ*).

## II. Phonetic Hard-Coding & Semantic Distinctions
Strict adherence to these phonetic laws is required for database consistency and script synchronization.

### 1. The Mahāprāṇa (Aspiration) Constraint
Aspirated consonants (**dh, bh, kh, th, gh**) carry distinct semantic value and must **never** be collapsed into their unaspirated counterparts.
* **Semantic Near-Misses:** Words that sound nearly identical must be treated as distinct lexical entries.
    * *mukau* (मुकौ — silent/mute dual) vs. *mukhau* (मुखौ — mouth/face dual).
    * *dhaukau* (धौकौ) is a unique semantic entity and is not a typo for *daukau*.

### 2. Consonant Fluidity
* **The Y-Shift:** In the absence of a hard "J," sounds beginning with *Y* may correspond to either *J* or *Y* in the source lexicon (e.g., *yāne* vs *jāne*).
* **The B/V/W Interchange:** The consonants *B*, *V*, and *W* are treated as interchangeable within the spoken Prakrit and Marathi series.

## III. Grammatical & Functional Markers (The Anchors)

### 1. The Verb "To Be" (Ho)
* **Rule:** The syllable **Ho** (हो) functions as the primary **Verb to Be** (is/are/become) or as an affirmative particle.
* **Usage:** It frequently appears at the end of clauses to stabilize the identity of the subject.

### 2. The Lunar Mansion Alignment (Animal Symbolism)
* **Rule:** Any animal reference (e.g., Horse/Yāradā, Elephant/Radah, Serpent/Ḍhau, Antelope/Ruī) must be cross-referenced against the **Sanskrit Zodiac (Nakshatras/Lunar Mansions)**.
* **Application:** These terms provide the astronomical or temporal context for the verse rather than simple description.

### 3. Suffix Anchors
| Suffix | Grammatical Function | Contextual Significance |
| :--- | :--- | :--- |
| **-a** | **Singular** | Primary subject or agent. |
| **-au / -ou** | **Sanskrit Dual** | Denotes "The Two" (e.g., The Maruts, Paired Emissaries). |
| **-ah / -as** | **Plural / Nominative** | Denotes a collective body or the primary actor. |

## IV. Data Standards & Workflow
* **Encoding:** **UTF-8-SIG (BOM)** is mandatory for all CSV and JSON exports to maintain Devanagari integrity.
* **The Pipeline:**
    1. **Extraction:** Raw phonetic transcription of audio.
    2. **Alignment:** Cross-reference against `lexicon_master.csv` and **Nakshatra** symbols.
    3. **Syntax Mapping:** Apply the **Ho-Verb** and Suffix rules to determine verse structure.
    4. **Commitment:** Update the **Book of Record** only after phonetic and grammatical laws are satisfied.
