# The Bullshitzky Institute — Approved Research

This **public repository** contains approved, published fictional research for [The Bullshitzky Institute](https://bullshitzky-institute.eliaselhage.workers.dev/).

## Research Studio publishing instructions

The **only** publication data file is [research.json](./research.json). It is read by the Institute website, which merges valid records with the six original findings. This repository has no access to the website's private source code, reader comments, or the owner's other accounts.

After the contributor reviews the exact final text and explicitly says **Publish**:

1. Read the current `research.json` from the `main` branch. Never use an earlier copy as a replacement.
2. Check the new article is not a duplicate. Create a unique lowercase hyphenated `slug` and choose one already approved `category`.
3. Append **one** research object under the `research` array. Preserve every existing research object verbatim, including its order, title, paragraphs, and metadata.
4. Do not change the `categories` map, README, code, or previously published research. Adding a new category or revising existing research needs separate owner approval.
5. Save `research.json` to this repository's `main` branch through the authorized GitHub connection. Do not access other repositories or connected accounts.
6. Re-read `research.json` to verify the record was saved. Check the public website when available. Report the publication honestly; changes may take a few minutes to appear because of caching.

## Research record format

Each item in the JSON `research` array follows this structure:

```json
{
  "slug": "a-unique-kebab-case-slug",
  "title": "Exact approved title",
  "type": "Micro Finding",
  "category": "relationships",
  "paragraphs": [
    "Exact approved first paragraph.",
    "Second paragraph with **optional bold emphasis**."
  ]
}
```

Valid content types are **Micro Finding**, **Standard Finding**, **Bullshitzky Commentary**, and **Institute Communication**. Choose the appropriate type using the Research Studio's approved Content System guide. The existing category codes are recorded in the `categories` map in `research.json`. A contributor cannot authorize new categories by adding new codes to a post.

Each paragraph must preserve the approved words exactly. Bold emphasis can be encoded using `**text**`. Never include private or personal account information in this public repository.

## Publication status

The six original approved findings have been copied here verbatim. New research belongs in the same `research` array. The website periodically reads this feed from GitHub; no Cloudflare or website-code edits are needed to publish a valid item in an existing approved category.

## Safety boundary

This repository is a **public research content store**, not a vault for drafts, passwords, keys, private conversations, or Strategic Streamline documents. The Research Studio must not edit the website's source-code repository.
