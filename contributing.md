# Contribution Guidelines

First of all, thanks for taking the time to contribute to this project!

## Submitting issues

- Ensure the issue was not already reported by searching on GitHub under issues.
- If you're unable to find an open issue addressing the problem, open a new one. Be sure to include a title and clear description, as much relevant information as possible.

## Submitting pull requests

- [ ] Ensure the PR description clearly describes the VS Code settings you are adding or changing.
- [ ] Include the relevant issue number if applicable.
- [ ] Ensure your changes are formatted correctly.

## Adding a new VS Code setting

Want to add a new VS Code setting to this repo? Follow these steps.

### Step 1: Pick the right section in `readme.md`

Open `readme.md` and find the category where your setting belongs.

Examples:

- `Editor`
- `Explorer`
- `Search`
- `Source Control`
- `Testing`
- `Terminal`
- `User Interface`

If there is no suitable category, you can create a new one.

### Step 2: Update the table of contents

In the `Contents` section at the top of `readme.md`:

- Add the main category if it does not already exist.
- Add your VS Code setting under that category.

Example:

```md
- [Testing](#testing)
  - [Never Auto-Open Test Results](#never-auto-open-test-results) - Prevent the Testing view from opening automatically.
```

#### How TOC links work

Convert the heading text into a lowercase anchor with hyphens.

Example:

- `### Never Auto-Open Test Results`
- becomes `#never-auto-open-test-results`

### Step 3: Add the new setting section

Under the correct category in `readme.md`, add your setting using this format:

````md
### Setting Title

#### Overview

Explain what this VS Code setting does and what problem it solves.

#### How to Solve the Issue

Explain when to use it, why it is useful, and any caveats if needed.

#### Setting

```json
"your.setting.name": true
```
````

You can also add:

- an example
- a screenshot
- an official VS Code source link

### Step 4: Keep the wording simple

Please keep the content clear and appropriately detailed for the setting.

### Step 5: Prefer official sources

If possible, link to:

- official VS Code documentation
- official VS Code release notes
- official Microsoft source references

Avoid unclear or low-quality sources when better official references exist.

### Step 6: Check everything before submitting

Before opening a pull request, make sure:

- the setting is added in the correct section
- the table of contents includes the new entry
- the anchor link matches the heading
- the JSON setting is valid
- the text is formatted correctly
