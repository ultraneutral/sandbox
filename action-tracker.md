## Purpose of this document

- Tracability of high level tasks requiring synchronized effort of multiple team members
- Documenting project decisions impacting multiple subsystems or team members
- It is NOT a task list for day to day work replacing Asana or Trello

## Format

The document is markdown in GFM (Github Flavored Markdown) style.
File revisions are stored in Github repository to preserve history (and because devs are working anyway with it).

Each entry consists of headline, an optional short description and an optional action item list.

### Headline

[Action Date] - [Category] - [Summary] ([Owner])

- Action Date: Required. Latest time an item must be reviewed (Either a deadline or validation of item)
- Category: Optional. Dependency, Obstacle/Impediment, Risk ... (add more if required)
- Summary: Required. Short description of item (less than 60 characters)
- Owner: Required.

### Description (Optional)

Just a plain text. Each amendment and the initial text block should be followed by a datestamp and optional author to make change history visible.

### Action Item List (optional)

Consists of itemized list (can use - [ ]) with action date, owner and description. If required a description of the outcome of an action item can be added to the description.

## Example

### 2016-05-09 - Impediment - Add new time travel library (hgwells)

Our current time travel API generates fluctuations in the sub space matrix which we must get rid off. [2016-05-01 hgwells]
Research shows we have a problem in the flux compensator. [2016-05-07 hgwells]

- [x] 2016-05-06 hgwells: Check if flux compensator causes the problem
- [ ] 2016-05-09 hgwells: Evaluate other time travel APIs

### 2016-09-01 - Risk - The lead to gold plugin might not be ready in time (midas)

### 2016-07-01 - Dependency - Library B needs config files from C library (cody)

We can't start with B library unless at least the config files are defined and implemented in C library. [2016-05-01 cody]

- [ ] 2016-07-01 smithy Re-evaluate situation
