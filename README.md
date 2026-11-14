# Setting up licensing for a new repo

This template follows **NOAA Handbook for Release of Software – Documenting License Files**. Software developed by NOAA employees or with NOAA funding is to be released via an open source license per the [NAO 201-118: SOFTWARE GOVERNANCE AND PUBLIC RELEASE POLICY](https://www.noaa.gov/administration/nao-201-118-software-governance-and-public-release-policy).

Each repo should include:

Every repo gets two licenses: **Apache 2.0** for source code (`LICENSE.md`) and
**CC0 1.0** for documentation and data (`LICENSE-DOCS.md`). `LICENSE.md` stays the
primary license so GitHub detects it; the Scope section of `NOTICE` says which
license covers what.

Pick your case below and copy that variant's `NOTICE` and `INTENT.md` into the
repo root, replacing the ones there. Then make the `LICENSE.md` change listed,
fill in the placeholders, and delete this `variants/` folder.
The default files at the repo root are for the all-federal case. In that does not apply, replace with the appropriate variant in the `variants/` folder and then delete the folder.

## 1. Pick your case

| Who wrote the code? | License | Variant folder | `LICENSE.md` change |
|---|---|---|---|
| **Federal employees only** (default) | Apache-2.0 (or another OSI-approved permissive license if contributing to an existing project) | `variants/federal/` | None; fill in `[YEAR]` |
| **Contractor** | Apache-2.0 unless the contract names another or the Contracting Officer approves one | `variants/contractor/` | Replace the top copyright line with the one from `NOTICE` |
| **Grantee / Cooperative Institute** | Apache-2.0 unless the agreement names another or the Grants Officer approves one | `variants/grantee/` | Replace the top copyright line with the one from `NOTICE` |
| **Other partner** (CRADA, MOU, OTA, international) | Whatever the agreement specifies | `variants/partner/` | Replace the whole file with that license if it isn't Apache-2.0 |
| **Joint federal + external** (inseparable contributions) | Apache-2.0 unless the agreement names another | `variants/joint/` | Replace the top copyright line with the one from `NOTICE` |

## 2. Fill in the placeholders

Search the repo for bracketed placeholders:

```bash
grep -rn "\[YEAR\]\|\[PROJECT NAME\]\|\[LINE OFFICE\|\[CONTRACT\|\[AWARD\|\[AGREEMENT\|\[INSTITUTION\|\[PARTNER\|\[EXTERNAL\|\[LICENSE\|\[SPDX\|\[choose" --exclude-dir=.git .
```

- `[YEAR]` is the year the software was developed. For multi-year work, use a range such as `2024-2026`.
- Leave the bracketed fields in the Apache **Appendix** of `LICENSE.md` as they are. They're part of the standard license text.

## 3. Third-party code

If the project includes third-party software, its licenses and copyright notices
**must be retained and reproduced** in any public release. Keep each original
license next to its code (or in a `THIRD_PARTY/` folder), and list every
component in the "Third-party software" section of `NOTICE`.

## 4. README

Paste this into the project README and edit it for your case:

```markdown
## License

Source code in this project is licensed under the [Apache License 2.0](LICENSE.md).
Documentation and data is dedicated to the public domain under [CC0 1.0](LICENSE-DOCS.md).
See [NOTICE](NOTICE) for copyright and attribution details, and
[INTENT.md](INTENT.md) for how U.S. copyright law applies to work by
federal employees.
```
