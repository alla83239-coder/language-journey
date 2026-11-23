# Insight source library

## Scope

Source root on the user's computer:

`D:\\Учебные материалы\\Insight\\insight 2022`

Five course folders were inventoried recursively on 24 November 2026. The full file-level CSV inventory is retained on the source computer as `Insight_Master_Inventory.csv`.

| Folder | Working CEFR range | Files found | Approx. size |
|---|---:|---:|---:|
| Elementary | A1–A2 | 286 | 1.97 GiB |
| Pre_Int | A2–B1 | 170 | 2.94 GiB |
| intermediate | B1–B2 | 45 | 1.46 GiB |
| Upper-Intermediate | B2–C1 | 13 | 0.96 GiB |
| Advanced | C1–C2 | 14 | 1.13 GiB |
| **Total** | **A1–C2** | **528** | **8.46 GiB** |

Counts include files inside extracted folders, not just archives. Some archives duplicate extracted resources, so these counts are a source inventory, not a count of unique learning assets.

## Resource types observed

- Student's Books and Workbooks (PDF)
- Grammar Reference and Practice
- Wordlists and exam answer keys
- Teacher's Guides
- Communication Worksheets and answer keys
- Documentary Video units and worksheets
- Global Skills videos and worksheets
- Student's Book and Workbook audio archives
- Pronunciation Insight worksheets and audio
- Interactive HTML/ZIP projects developed for the course

## Important source-library notes

- **Pre_Int** includes the dedicated *Welcome to my world* source pack, its Student's Book, Teacher's Book, Workbook, grammar reference, audio, worksheets, videos and several successive web-app prototypes. It also contains *Spoiled for Choice* source PDFs and the existing game.
- **Elementary** includes multiple project versions of *You are what you eat*. These must be compared before selecting the canonical build.
- Some levels have both extracted folders and RAR/ZIP archives containing the same assets. Do not import both copies blindly.
- The separate `Для занятий` folder is outside the five course folders and has not yet been included in the 528-file count. It will be inventoried as a separate supplementary collection.
- Several upper-level audio/video resources are present only as archives. Archive contents must be mapped to units before the media are linked to modules.

## Repository import policy

The source library is approximately 8.46 GiB. Do not copy the entire raw library into the ordinary Git repository. The repository should contain:

1. source manifests, unit/topic maps and attribution/source references;
2. only the media needed by active web modules, optimized for web delivery;
3. original large PDFs, RAR/ZIP archives and full-length videos kept in the user's source library or a suitable file/object store;
4. stable relative asset references in course data, with missing-asset checks.

This avoids repository size limits, repeated archives and broken media paths.

## Curriculum rule

The five courses are one continuous progression, not five unrelated syllabi. Each topic must have a vertical map from Elementary through Advanced, with increasing lexical range, grammatical control, discourse complexity, critical thinking and project demands. A topic's appearance in a higher level must extend prior learning rather than simply repeat it.

## Next source-analysis steps

1. Confirm the canonical Student's Book, Workbook and Teacher's Guide in each folder.
2. Extract unit titles, reading/listening themes, vocabulary fields, grammar and writing/speaking outcomes from the source books and guides.
3. Map supplementary media and worksheets to their exact units.
4. Build the cross-level topic matrix.
5. Derive five level-specific thematic plans from that matrix.
6. Only then populate the interactive modules using the Spoiled for Choice gameplay engine.
