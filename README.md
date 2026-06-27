# apologia

A bilingual evangelical-Protestant apologetics **field reference**, typeset with the
[texish](https://github.com/edadma/texish) document engine. It comes in two editions:

- **French / English** — `apologia-fr-en.texish`
- **Spanish / English** — `apologia-es-en.texish`

The document is a deck of one-page "cards," each answering a common question or objection
with a short answer, a few key points, and the scripture printed in full so it can be read
straight from the page. It is laid out for a small half-letter booklet (5.5 × 8.5 in): the
other-language take of each card sits on the left (verso) page and the matching English take on
the right (recto), so the two languages always face each other. A trilingual cover (Greek title
*Ἀπολογία* with the two subtitles) and separate tables of contents open the book; the cover
carries the full date as a version stamp.

Scripture is quoted from public-domain translations — the **Berean Standard Bible** in English,
**Louis Segond 1910** in French, and the **Reina-Valera 1909** (modernized) in Spanish.

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
./cli/target/scala-3.8.4/texish-cli /path/to/apologia/apologia-fr-en.texish   # French / English
./cli/target/scala-3.8.4/texish-cli /path/to/apologia/apologia-es-en.texish   # Spanish / English
```

This writes the PDF beside the source (`apologia-fr-en.pdf`, `apologia-es-en.pdf`). Rendered PDFs
are not tracked in this repository.

A ready-to-print PDF of the latest version is attached to the most recent
[GitHub release](https://github.com/edadma/apologia/releases). Releases are versioned by the
cover date (tag `v<YYYY.MM.DD>`), which doubles as the document version.

## License

This work is dedicated to the public domain under
[CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) — see [`LICENSE`](LICENSE).
Copy, modify, distribute, and print it freely, even commercially, without asking permission.

Scripture is quoted from public-domain translations: the **Louis Segond 1910** (French) and the
**Berean Standard Bible** (English).
