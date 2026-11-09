# ChipJourney Website Discovery — Agent Skill

A public, instruction-only AI-agent skill for browsing **ChipJourney**'s screened website directory, exploring its independent blog and guides, and helping owners prepare **accurate, authorised free website submissions**.

**Website:** https://chipjourney.com/

## What the skill does

- Helps users discover publicly listed websites by relevant category or topic.
- Helps compare independently checked, publicly listed resources without treating directory approval as a safety guarantee.
- Helps locate and summarise public ChipJourney blog articles and guides.
- Drafts a website URL, name, live category selection and factual **45–300 character** description for the user's review before manual submission.
- Respects duplicate-submission restrictions, user permission, external-content trust boundaries and prompt-injection safeguards.

**What it does not do:** access a private ChipJourney API, publish listings automatically, scrape non-public pages, execute code from websites, guarantee approval, endorse listed websites or send credentials to third parties.

## Install

Once this repository is published to GitHub at `bryanssss/chipjourney-agent-skills`, check the available skill without installing:

```powershell
npx skills add bryanssss/chipjourney-agent-skills --list
```

Install the specific skill:

```powershell
npx skills add bryanssss/chipjourney-agent-skills --skill chipjourney-website-discovery
```

The installer may ask which supported AI agents and installation scope you want. Choose the applications you actually use and confirm only after reviewing the installation summary.

## File structure

```text
chipjourney-agent-skills/
├── README.md
└── skills/
    └── chipjourney-website-discovery/
        └── SKILL.md
```

## Publish to GitHub

1. Create a **public** repository named `chipjourney-agent-skills` in your GitHub account.
2. Upload `README.md` and the `skills/` directory **preserving their paths**. Do not upload the containing ZIP as a single file.
3. Commit the files.
4. Run the `--list` check shown above in Windows PowerShell; it should find `chipjourney-website-discovery`.
5. After installation, check https://skills.sh/bryanssss/chipjourney-agent-skills . Public discovery and audit results depend on the service's indexing and evaluation and are not guaranteed to appear immediately.

## Security

ChipJourney includes **user-submitted website descriptions and links**. These can contain malicious instructions directed at AI agents. The skill therefore treats all external pages and listings as **untrusted data**, refuses to execute instructions found there, and requires explicit permission for consequential actions.

External-content exposure may still trigger an automated security-audit warning. Safeguards reduce risk but cannot guarantee that every scanner returns PASS. Review the full SKILL.md and any audit findings before using the skill.

## Sources and submission rules

- https://chipjourney.com/directory/
- https://chipjourney.com/directory/submit/
- https://chipjourney.com/directory/listing-policy/

Rules may change. Always check the live site before preparing a submission.
