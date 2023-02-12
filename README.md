# licenses.markdown

Licenses in Markdown format.

These are licenses I regularly use in my projects, in Markdown format.

- CC-BY-4.0
- CC-BY-SA-4.0
- CC0-1.0
- MIT-0
- MIT
- MPL-2.0
- ODC-By-1.0
- ODC-DbCL-1.0
- ODC-ODbL-1.0

## Filename formats

All filenames are in this format: `code.markdown`. If there is a summary available, the license itself has a suffix of `-legal` while the human-readable version with `-summary`.

Examples:

- `MIT.markdown`
- `MIT-0.markdown`
- `CC-BY-SA-4.0-legal.markdown`
- `CC-BY-SA-4.0-summary.markdown`

### Notes

1. Only the legal version is required to be included in your project.
1. The traditional naming scheme are: `LICENSE`, `LICENSE.txt`, `LICENSE.md`, or `LICENSE.markdown`.
    - Since these files are in Markdown, only use `LICENSE.md` or `LICENSE.markdown`.
    - Traditionally, this file contains the primary license of your repository.
      - If it is software, it contains a software license.
      - If your repository is for blog articles, images, or music sheets, to mention a few, it should have a license applicable for works of art.
1. If you want to include the human-readable version, if any, this is how I do it:
    - For the legal: `LICENSE.md` or `LICENSE.markdown`
    - For the summary: `LICENSE-summary.md` or `LICENSE-summary.markdown`
1. If there are multiple licenses in your project—a separate license for the software binary and code; and another for works of art (images, documentation, keyboard layouts, content)—there are different ways of arranging your licenses.
    - Method 1: One `LICENSE.markdown` file
      - Include both legal codes in the same file. Add a note at the top clarifying which license applies to which part of your work.
    - Method 2: Separate licenses
      - `LICENSE.markdown`
      - `LICENSE-documentation.markdown`
      - `LICENSE-summary-software.markdown`
      - `LICENSE-legal-content.markdown`
      - `LICENSE-summary-content.markdown`

## Contribute

If you are interested in contributing to this repository, please open a PR.

Our primary repository is at [Codeberg](https://codeberg.org/yelosan/licenses.markdown).

Mirrors/Backup are:

- [GitLab](https://gitlab.com/yelosan/licenses.markdown)
- [GitHub](https://github.com/yelosan/licenses.markdown)

### Guidelines

1. The top information should contain the following:

    ```markdown
    # Attribution 4.0 International (CC-BY-4.0)

    (Copied from [Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/legalcode) and converted to markdown on 2023-02-12.)
    ```

    - The first heading is the actual name of the license.
    - The SPDX license code, if any, should be in parenthesis "()".
    - A note when it was copied in ISO date notation (YYYY-MM-DD), and a link to the original source.
      - If there is no available original page, for example, MIT, a link to SPDX will suffice.

1. Convert the original text as close as possible.

    - If a text appears to be a quote/blockquote, convert it into Markdown as a quote/blockquote.
    - If in the original they used Arabic or Roman numerals for ordered lists, keep the same in Markdown.
      - There might be instances when an exact duplication is not possible due to Markdown parsing. Find the closest format as possible and be consistent in the rest of the document.
    - In the Markdown file, use the actual ordering. Do not use all "1." (which Markdown converts accordingly), instead use, "1.", "2.", "3." This way, if someone opens the Markdown file itself, it still is clear to the reader.

1. If in doubt, check existing license files.
