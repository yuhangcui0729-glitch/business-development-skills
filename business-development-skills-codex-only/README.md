# Business Development — Three Coaching Skills for Codex (EN/DE)

Three student-led workshops for Business Development (2026W), available in **English or German**:

1. **Business Model Canvas Coach** — develop a first canvas and question your assumptions.
2. **Market & Marketing Coach** — SWOT, competitors, positioning, and the marketing mix.
3. **Finance & Legal Issues** — costs, pricing, sales assumptions, funding, and Austrian legal considerations.

[Deutsche Anleitung](README.de.md)

## Student instructions: install in Codex

**Requirements:** Access to a Codex application/environment that supports skills and the `$skill-installer` skill, plus internet access to GitHub. These instructions are for **Codex**, not the ordinary ChatGPT Skills interface. Availability depends on the account and Codex client.

1. Open **Codex** and start a new conversation.
2. Send each of the following messages **in the Codex chat** (not in your computer's terminal). Replace `YOUR-USERNAME` with the GitHub username or organization that hosts this repository; change `business-development-skills` if the actual repository has a different name.

   **Workshop 1 — Business Model Canvas**

   ```text
   $skill-installer install https://github.com/YOUR-USERNAME/business-development-skills/tree/main/skills/business-model-canvas-coach
   ```

   **Workshop 2 — Market & Marketing**

   ```text
   $skill-installer install https://github.com/YOUR-USERNAME/business-development-skills/tree/main/skills/market-and-marketing-coach
   ```

   **Workshop 3 — Finance & Legal Issues**

   ```text
   $skill-installer install https://github.com/YOUR-USERNAME/business-development-skills/tree/main/skills/finance-and-legal-issues
   ```

3. **Restart Codex** after installing so the skills become available. You need to install each skill only once, unless its instructions are updated.
4. Start **a separate conversation for each workshop**, using the same venture idea throughout. To activate a skill, explicitly name it:

   ```text
   Use the business-model-canvas-coach skill. Let's go!
   ```

   Then, in the next workshop:

   ```text
   Use the market-and-marketing-coach skill. Let's go!
   ```

   And finally:

   ```text
   Use the finance-and-legal-issues skill. Let's go!
   ```

   To work in German, replace `Let's go!` with `Los geht's!`. At the start of workshops 2 and 3, provide the preceding workshop's final summary.
5. Respond to the coach using your own reasoning. You can challenge suggestions, explain a different idea, or advance to the next step. **Follow the examination instructions on Moodle** for the required submission and reflection.

**If installation does not work:** Verify that the repository is public, the link contains the correct GitHub username, and your Codex client supports `$skill-installer`. Some Codex environments differ; the command is not a shell command to run in Terminal. If a skill with the same name is already installed, consult Codex's instructions for updating it.

**Note on submissions:** Check whether the Codex client you use lets you share a complete conversation. Do not assume its sharing features are identical to ChatGPT. Confirm the submission method with the course instructor if necessary.

## Repository structure

```text
business-development-skills/
├── README.md
├── README.de.md
└── skills/
    ├── business-model-canvas-coach/
    ├── market-and-marketing-coach/
    └── finance-and-legal-issues/
```

Each skill folder includes `SKILL.md`, supporting `references/`, and assets. Keep the entire folder intact when installing.

## For the course instructor: publish on GitHub

1. Create a **public** repository at https://github.com/new, for example `business-development-skills`.
2. Do not initialize the repository with an additional README.
3. Extract the repository ZIP and upload the **contents** (both READMEs and the `skills/` folder), then commit.
4. Replace `YOUR-USERNAME` in the three example commands above with your actual GitHub username or organization before sharing the repository with students.

## Permissions and privacy

No license has been added. Before making the repository public, review the materials and image rights and decide whether to add a license allowing reuse. Keep students' conversations and submissions out of this repository.

Codex installer reference: [OpenAI skill installer](https://github.com/openai/skills/blob/main/skills/.system/skill-installer/SKILL.md).
