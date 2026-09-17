# ESL — Source Hub

This page is the exhaustive discovery entry for the product's currently synchronized local sources. Read it before answering any ESL / electronic shelf label / F24A7 base-station question.

The canonical product root is **ESL**: a size-variant electronic shelf-label family plus the matching 2.4 GHz base station. There is no combined series spec occupying the single `specs/` slot. Size-specific specs and the base-station spec live under `others/`.

## Current Source Coverage

| Type | Document key | Document | Markdown | Original |
| --- | --- | --- | --- | --- |
| presentation | `overview-en_202608182031` | UROVO Electronic Shelf Labels Overview | `ESL/presentation/overview-en_202608182031/ESL-Presentation-EN-0514.md` | `ESL/presentation/overview-en_202608182031/ESL-Presentation-EN-0514.pptx` |
| others | `spec-2.1inch_202608182031` | 2.1-inch series ESL spec (ET0213) | `ESL/others/spec-2.1inch_202608182031/ESL-2.1inch-Specs.md` | `ESL/others/spec-2.1inch_202608182031/ESL-2.1inch-Specs.docx` |
| others | `spec-2.6inch-t2664_202608182031` | T2664 2.66-inch ESL spec | `ESL/others/spec-2.6inch-t2664_202608182031/ESL-2.6inch-Specs.md` | `ESL/others/spec-2.6inch-t2664_202608182031/ESL-2.6inch-Specs.docx` |
| others | `spec-4.2inch_202608182031` | 4.2-inch series ESL spec (ET0420) | `ESL/others/spec-4.2inch_202608182031/ESL-4.2inch-Specs.md` | `ESL/others/spec-4.2inch_202608182031/ESL-4.2inch-Specs.docx` |
| others | `base-station-spec-en_202608182031` | F24A7 ESL Base Station Specification | `ESL/others/base-station-spec-en_202608182031/ESL_Base_Station_Specification_EN.md` | `ESL/others/base-station-spec-en_202608182031/ESL_Base_Station_Specification_EN.pdf` |

A previous 1.6-inch tag-spec input was not synchronized because it was not a valid DOCX/PDF/OLE document; that failed input is no longer present in the inbox. The English overview names a **1.54-inch** size that currently has no synchronized spec.

## Vault Knowledge

- [[spec/ESL|ESL Specification]]
- [[pb/ESL|ESL Brochure / Product Page]]
- [[categories/esl|Electronic Shelf Labels]]

## Shared Knowledge

No synchronized multi-product source is currently linked.

## Active Local Source Discrepancies

| Field | Values | Sources | Status |
| --- | --- | --- | --- |
| Tag battery life | Presentation: 15 years (slide 4; slide 7 also says 600 mA, twice-daily refresh, 15 years on the 2.66-inch module). 2.1-inch spec: CR2450 × 2, 不低于7年. 4.2-inch spec: CR2450 × 3, 不低于7年. T2664 spec: 内置电池×2, no year figure. | `ESL/presentation/overview-en_202608182031/ESL-Presentation-EN-0514.md` vs `ESL/others/spec-2.1inch_202608182031/ESL-2.1inch-Specs.md` vs `ESL/others/spec-4.2inch_202608182031/ESL-4.2inch-Specs.md` vs `ESL/others/spec-2.6inch-t2664_202608182031/ESL-2.6inch-Specs.md` | Unresolved. Size and refresh-rate conditions differ; do not merge. |
| Tag IP rating | Presentation slides 4 and 21: IP68. Slide 7 assigns IP68 to the 83×42×12 mm / 2.66-inch block. 2.1-inch and 4.2-inch specs: IP65 default, IP68 optional. T2664 spec does not list IP. | presentation vs 2.1-inch spec vs 4.2-inch spec vs T2664 spec | Unresolved |
| Tag RF range | 2.1-inch and 4.2-inch specs: 30 m (50 m open). T2664 spec and presentation slides 7/9: 100 m (base-station antenna / power dependent). | 2.1-inch spec / 4.2-inch spec vs T2664 spec / presentation | Unresolved; may be size-line differences |
| Viewing angle | Presentation slide 8: 180°. 2.1-inch and 4.2-inch specs: >170°. T2664 spec has no viewing-angle row. | presentation vs 2.1-inch spec vs 4.2-inch spec | Unresolved |
| Phone management without base station | 2.1-inch spec advantages: NFC. 4.2-inch spec advantages: Bluetooth. Presentation: Built-in NFC as standard. 2.1/4.2 feature tables: NFC optional. | 2.1-inch spec vs 4.2-inch spec vs presentation | Unresolved |
| Base station Wi-Fi | F24A7 PDF p.4 advantages: 100M Ethernet and WIFI. PDF p.5 Network Support: Ethernet only. Presentation base-station slides list Ethernet, not Wi-Fi. | `ESL/others/base-station-spec-en_202608182031/ESL_Base_Station_Specification_EN.md` p.4 vs p.5 vs presentation | Unresolved |
| Base station dimensions | Spec table: 150×95.5×23.8 mm (may have slight error). Drawing: 150.20×95.20×23.50 mm | same F24A7 PDF table vs drawing | Unresolved; drawing vs rounded table |

## Query Coverage Rule

- Treat the source table above as the complete discovery set for this product.
- Route size-specific hard specs to the matching `others` spec. Route positioning, sizes, platform, and deployment to the presentation. Route F24A7 hardware to the base-station spec.
- For a broad or exhaustive request, read every listed Markdown source.
- If routing remains uncertain, search all Markdown under `ESL/` before concluding that information is unavailable.
- Always surface a relevant row from Active Local Source Discrepancies instead of choosing a winner.
