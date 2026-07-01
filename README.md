# apologia

A bilingual evangelical-Protestant apologetics **field reference**, typeset with the
[texish](https://github.com/edadma/texish) document engine. It comes in nine editions:

- **French / English** — `apologia-fr-en.texish`
- **Spanish / English** — `apologia-es-en.texish`
- **Portuguese / English** — `apologia-pt-en.texish`
- **Simplified Chinese / English** — `apologia-zh-hans-en.texish`
- **Traditional Chinese / English** — `apologia-zh-hant-en.texish`
- **Hindi / English** — `apologia-hi-en.texish` (Devanagari)
- **Bengali / English** — `apologia-bn-en.texish` (Bengali–Assamese script)
- **Hebrew / English** — `apologia-he-en.texish` (right-to-left)
- **Arabic / English** — `apologia-ar-en.texish` (right-to-left)

The document is a deck of one-page "cards," each answering a common question or objection
with a short answer, a few key points, and the scripture printed in full so it can be read
straight from the page. It is laid out for a small half-letter booklet (5.5 × 8.5 in): the
other-language take of each card sits on the left (verso) page and the matching English take on
the right (recto), so the two languages always face each other. A trilingual cover (Greek title
*Ἀπολογία* with the two subtitles) and separate tables of contents open the book; the cover
carries the full date as a version stamp.

Scripture is quoted from public-domain translations — the **Berean Standard Bible** in English,
**Louis Segond 1910** in French, the **Reina-Valera 1909** (modernized) in Spanish, the **Bíblia
Livre** (a public-domain corrected Almeida) in Portuguese, the **Chinese Union Version** (和合本,
1919) in Chinese (Simplified and Traditional script), in Hebrew, the **Salkinson-Ginsburg Hebrew New
Testament** (1885) with the **Westminster Leningrad Codex** for Old Testament quotations, and, in
Arabic, the **Smith–Van Dyck Bible** (1865). The Hindi and Bengali editions have no suitable
public-domain modern Bible to draw on, so their verses are an **original translation from the Hebrew
and Greek**, likewise dedicated to the public domain.

## Contents

The deck is organized under five broad sections:

| Section | Cards |
|---|---|
| Sharing the Gospel | Opening questions · The good news · Leading to faith |
| God | Evidence and science · Why suffering |
| The Bible | Contradictions and transmission · Evolution |
| Jesus | Good teacher and resurrection · All roads to God |
| The human heart | Good, and good enough · Hypocrites |

## Building

Each edition is a self-contained texish document. Render one to PDF from a texish checkout
(fonts load relative to the working directory):

```sh
cd /path/to/texish
./cli/target/scala-3.8.4/texish-cli /path/to/apologia/apologia-fr-en.texish      # French / English
./cli/target/scala-3.8.4/texish-cli /path/to/apologia/apologia-es-en.texish      # Spanish / English
./cli/target/scala-3.8.4/texish-cli /path/to/apologia/apologia-pt-en.texish      # Portuguese / English
./cli/target/scala-3.8.4/texish-cli /path/to/apologia/apologia-zh-hans-en.texish # Simplified Chinese / English
./cli/target/scala-3.8.4/texish-cli /path/to/apologia/apologia-zh-hant-en.texish # Traditional Chinese / English
./cli/target/scala-3.8.4/texish-cli /path/to/apologia/apologia-hi-en.texish      # Hindi / English
./cli/target/scala-3.8.4/texish-cli /path/to/apologia/apologia-bn-en.texish      # Bengali / English
./cli/target/scala-3.8.4/texish-cli /path/to/apologia/apologia-he-en.texish      # Hebrew / English
./cli/target/scala-3.8.4/texish-cli /path/to/apologia/apologia-ar-en.texish      # Arabic / English
```

This writes the PDF beside the source (`apologia-fr-en.pdf`, `apologia-es-en.pdf`,
`apologia-pt-en.pdf`, `apologia-zh-hans-en.pdf`, `apologia-zh-hant-en.pdf`, `apologia-hi-en.pdf`,
`apologia-bn-en.pdf`, `apologia-he-en.pdf`, `apologia-ar-en.pdf`). Rendered PDFs are not tracked in
this repository. The Chinese editions need texish ≥ 0.11.1 (bundled Noto Serif CJK with a bold
weight); the Hebrew and Arabic editions need texish ≥ 0.13.1 (right-to-left Hebrew and Arabic with
vocalization, and right-to-left lists); the Portuguese edition needs texish ≥ 0.14.0 (bundled
Portuguese hyphenation) and the Hindi edition needs texish ≥ 0.14.0 (Devanagari shaping); the Bengali
edition needs texish ≥ 0.15.0 (Bengali–Assamese script shaping).

A ready-to-print PDF of the latest version is attached to the most recent
[GitHub release](https://github.com/christian-evangelism-media/apologia/releases). Releases are versioned by the
cover date (tag `v<YYYY.MM.DD>`), which doubles as the document version.

## License

This work is dedicated to the public domain under
[CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) — see [`LICENSE`](LICENSE).
Copy, modify, distribute, and print it freely, even commercially, without asking permission.

Scripture is quoted from public-domain translations (see above); the Hindi and Bengali verses are an
original translation from the Hebrew and Greek, also dedicated to the public domain.
