
# Content Rules & Criteria

This document defines **mandatory rules** for maintaining `index.json` and adding new educational content.

These rules exist to ensure:
- Offline-first reliability
- Safe content updates
- Backward compatibility
- Long-term stability for installed apps

All contributors **must follow these rules**.

---

## 1. `index.json` File (Authoritative Source)

`index.json` is the **single source of truth** for all content metadata.

### Required Structure

```json
{
  "version": 3,
  "last_updated": "2025-12-28",
  "items": [
    {
      "id": "android-network-monitor",
      "title": "Monitor Android Network Activity",
      "file": "android/network-monitoring.md",
      "level": "Intermediate",
      "platform": "Android"
    }
  ]
}

```

* * * * *

2\. Top-Level Field Rules
-------------------------

### `version`

-   Must be an **integer**

-   Must **increase** on every content change

-   Must never decrease or repeat

-   Used by the app to detect updates

**Do NOT reuse version numbers**

* * * * *

### `last_updated`

-   Must follow `YYYY-MM-DD` format

-   Must reflect the latest content change date

-   Informational only (not used for sync logic)

* * * * *

### `items`

-   Must be an array

-   Must never be empty

-   Each item represents one content entry

* * * * *

3\. Item Object Rules (Critical)
--------------------------------

Each object inside `items` **must follow these rules**:

| Field | Required | Rules |
| --- | --- | --- |
| `id` | ✅ | Unique, immutable, lowercase, hyphen-separated |
| `title` | ✅ | Human-readable, descriptive |
| `file` | ✅ | Relative path to markdown file |
| `level` | ✅ | `Beginner`, `Intermediate`, or `Advanced` |
| `platform` | ✅ | `Android`, `Windows`, `Linux`, `Email`, `Network`, `All` |

* * * * *

4\. ID Rules (IMMUTABLE)
------------------------

-   IDs are **permanent**

-   IDs must never be:

    -   renamed

    -   reused

    -   removed

-   IDs must be unique across the entire repository

### Allowed ID Format

```
lowercase-words-separated-by-hyphens

```

❌ Do not use spaces, underscores, or uppercase letters

* * * * *

5\. File Path Rules
-------------------

-   Must point to an existing `.md` file

-   Must be a **relative path**

-   Must match folder category

-   Once published, **file paths must never change**

### Example

```
"file": "android/network-monitoring.md"

```

❌ Do not move or rename published files

* * * * *

6\. Content Level Criteria
--------------------------

| Level | Criteria |
| --- | --- |
| Beginner | No prior technical knowledge required |
| Intermediate | Assumes basic IT/security knowledge |
| Advanced | Assumes professional experience |

* * * * *

7\. Platform Rules
------------------

-   Platform must reflect **primary target**

-   Use `All` only if content applies universally

-   Do not list multiple platforms in one field

* * * * *

8\. Markdown Content Rules
--------------------------

Markdown files must be:

### Allowed

-   Educational

-   Defensive

-   Configuration-based

-   Troubleshooting-focused

### Forbidden

-   Malware code

-   Exploits

-   Payloads

-   Offensive techniques

-   Reverse engineering steps

The app is **education-only**.

* * * * *

9\. Adding New Content (Required Steps)
---------------------------------------

1.  Create a new markdown file in the correct folder

2.  Add a new item entry in `index.json`

3.  Assign a **new unique ID**

4.  Increment `version`

5.  Update `last_updated`

6.  Commit and push

* * * * *

10\. Updating Existing Content
------------------------------

-   Modify markdown content only

-   Do **not** change:

    -   `id`

    -   `file`

    -   `level`

    -   `platform`

-   Increment `version` after updates

* * * * *

11\. Prohibited Actions (DO NOT DO)
-----------------------------------

❌ Delete items from `index.json`\
❌ Reuse or change IDs\
❌ Rename or move files\
❌ Decrease `version`\
❌ Add unsafe content

* * * * *

12\. Breaking Change Policy
---------------------------

Breaking changes are **not allowed**.

If content must be replaced:

-   Add a new item with a new ID

-   Mark old content as deprecated inside the markdown

* * * * *

13\. Responsibility
-------------------

-   Contributors must follow these rules

-   Maintainers must review all changes

-   App stability depends on strict compliance
