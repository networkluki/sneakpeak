# Public disclosure rules

This repository is **public**. Treat every file, attachment, issue, commit, branch, and pull request as potentially visible and permanently copied by third parties.

## Safe to publish

- General project themes, codenames, or already-public names.
- Reviewed screenshots with sensitive areas cropped or obscured **before upload**.
- Public-safe achievements described at a high level.
- Dated progress notes with no confidential roadmap details.
- Links to material that is already intended to be public.

## Do not publish

- Credentials, tokens, keys, environment files, database dumps, or personal data.
- Internal URLs, hostnames, IP addresses, admin interfaces, private repository links, or infrastructure diagrams.
- Vulnerability details or defensive blind spots that have not been responsibly resolved.
- Full code, unreleased algorithms, complete interfaces, or proprietary architecture.
- Internal issue IDs, private branch names, unannounced partnerships, or unapproved release dates.
- Original screenshots or source images that contain private data, even if a separately edited preview looks safe.

## Before every public commit

1. Write the teaser in a private scratch space outside this repository.
2. Confirm that the project or detail is approved for public disclosure.
3. Remove private metadata and check screenshot backgrounds, browser tabs, terminal history, tooltips, and file names.
4. Inspect the final files and the staged Git diff, including any binary attachments.
5. Verify that links point only to approved public resources.
6. Publish only the reviewed copy. When uncertain, leave the information out.

**Important:** `.gitignore` and deleting a later commit cannot reliably undo a public disclosure. Keep private source material in separate private repositories, not in hidden folders or branches here.

## Communication policy

- A status describes a public signal, not a promise.
- Never infer or invent project completion percentages.
- Avoid exact dates unless an official public date has already been decided.
- Do not auto-publish internal commit messages, issue titles, or private CI logs.
- Update previews selectively; silence is better than leaking confidential work.

[Back to Sneak//Peek](../README.md)
