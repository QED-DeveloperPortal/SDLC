---
index: true
---
# Contributions
This document explains **how to contribute, edit, review, and publish** updates to the SDLC documentation.
Our goal is to make the SDLC a **living, collaboratively maintained resource**, supported by subject-matter experts, delivery teams, and governance stakeholders.


## Purpose
- Provide clear instructions for contributing updates
- Explain how markdown files are structured and formatted
- Describe the contribution workflow (editing → review → approval)
- Identify roles and responsibilities (authors, guardians, approvers)
- Clarify how changes are tracked, reviewed, and released
- Encourage stewardship and ownership across specialist areas


# Working With Markdown
All SDLC documentation is stored in **Markdown (`.md`)**.
If you’re new to Markdown:
- It is a lightweight, text-based format
- Easy to edit in any Git tool or text editor
- Ideal for version control, code review, and automation


### Basic Markdown reference
````
# H1 Title
## H2 Heading
### H3 Subheading

**Bold text**  
*Italic text*  
> Blockquote  
- Bullet list  
1. Numbered list  

`inline code`

```code block```  
````
For a full Markdown reference, see:
[https://www.markdownguide.org/basic-syntax/](https://www.markdownguide.org/basic-syntax/)



# Editing tools
You may edit Markdown using any of the following:

### Web-based Git editors
- GitHub web editor (`.` hotkey)
- GitHub Desktop
- Azure DevOps Repos editor
- GitLab web IDE

### Local tools
- VS Code (recommended — with Markdown plugins)
- Sublime Text
- Atom
- Notepad++
- Any text editor of your choice

### Preview tools
- GitHub / GitLab built-in preview
- VS Code Markdown Preview (`Ctrl+Shift+V`)


# Contribution workflow
Contributions follow this simple workflow:
1. [Setup a GitHub.com account](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github)
1. [Fork the SLDC repo](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)
1. Use the [github.dev](https://docs.github.com/en/codespaces/the-githubdev-web-based-editor) online capability to make changes directly to your fork of the SDLC repo.
1. [Create a Pull Request](https://docs.github.com/en/codespaces/the-githubdev-web-based-editor#create-a-pull-request) to request that your modifications to the SDLC repo be merged into this main repo. Choose the main branch of the QED-DeveloperPortal/SDLC repo as where you want the changes merged to.
1. You will subsequently receive emails/notifications to confirm that your modifications have been accepted or any other communications about your Pull Request, such as suggested modifications raised by maintainers of the repo.
1. **Guardian review** (subject-matter expert)
1. **Approver sign-off** (owner of that SDLC section)
1. **Merge to main**
1. **Published automatically** to the developer.qed.qld.gov.au site.


# Guardians & approvals
Each major area of the SDLC should have **designated subject-matter guardians**.
A guardian is responsible for:
- Maintaining accuracy and currency of their assigned files
- Reviewing PRs that affect their domain
- Co-writing new guidance or clarifications
- Acting as the “first reviewer” for contributions
An approver:
- Has final authority to accept documentation changes
- Ensures alignment with policy/standards
- Coordinates content that affects multiple guardians


# Pull request expectations (PR)
When submitting changes:

### Please include:
- A short summary of what was updated and why
- Links to relevant issues or discussions
- Whether this is:
  * New content
  * A correction
  * A clarification
  * A modernisation update
  * A temporary supplement (to be moved into /supplementary)

### Guardians/approvers will check for:
- Accuracy and clarity
- Consistency with SDLC Tracks and Stages
- Compliance with standards
- Duplication or overlap with existing pages
- Impact on downstream processes or artefacts


# File structure & placement
When adding or updating content:
* Place files in the **appropriate Track → Stage → Process** folder
* Supplementary/tips content goes under:
  `/supplementary/`
* Templates should live under:
  `/artefacts/templates/`
* Large legacy or reference content lives under:
  `/appendices/`
If unsure, mention it in your PR description.


# Use of AI
Authors may use AI tools to assist in drafting, editing, or refining SDLC documentation.
However, any use of AI **must comply with Queensland Government AI guidance and all departmental policies**.
When using AI:
- Do not include personal, sensitive, confidential, or protected information** in prompts or inputs.
- Use Australian spelling, terminology, and grammar in all outputs.
- Review and verify the accuracy of all AI-generated content before submitting.
- Ensure all content complies with the SDLC, department standards, and relevant legislation.
AI can support efficiency and clarity, but **it does not replace human judgement**.
**Regardless of the source or process, *you* are responsible for the accuracy, appropriateness, and compliance of your contribution.**


# Testing and previewing your changes
Before submitting:
- Check Markdown formatting
- Preview changes using GitHub/DevOps or VS Code
- Run spellcheck (plugins recommended)
- Follow [Forgov.qld.gov.au](https://www.forgov.qld.gov.au/communication-and-publishing/website-standards-guidelines-and-templates/write-for-queensland-government-websites/web-writing-and-style-guide) writing standards
- Ensure headings and structure follow SDLC conventions
- Validate internal links (e.g., `[See Stage → Requirements](/tracks/track-1/stages/requirements/)`)


# Publishing
Once merged into the **main** branch:
* Your changes become part of the official SDLC repository
* Changes will appear **automatically** on the next build of developer.qed.qld.gov.au


# Feedback and Continuous Improvement
We welcome feedback and suggestions.
If you see areas where:
- Clarity is needed
- Additional examples would help
- Content is outdated
- Gaps exist in formal documentation
Please raise an Issue or start a discussion.


# Our goal
The SDLC is evolving.
Through contributions from delivery teams, architects, PMs, QA specialists, and product teams, we aim to create:
- Clearer
- Simpler
- More modern
- More usable
documentation for everyone.
Your contributions make that possible.


