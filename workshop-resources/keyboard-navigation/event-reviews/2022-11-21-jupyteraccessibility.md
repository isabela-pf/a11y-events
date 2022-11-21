# Collaborative keyboard navigation review

Please add your findings as [GitHub suggestions](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/commenting-on-a-pull-request) so you are credited in the commit history!

## Keyboard navigation accessibility review of [Jupyter accessibility documentation](https://jupyter-accessibility.readthedocs.io/en/latest/index.html)

Reviewed via based on [this link we'll all be working off of](https://jupyter-accessibility.readthedocs.io/en/latest/index.html).

- Review date:
- Operating system:
- Browser: 
- Keyboard language(s) used:
- Any other details (ie. dependencies, github repo, etc.):

### Authors and contents

- Content order: (add author(s))
- Areas to navigate: (add author(s))
- Keyboard/tab traps: (add author(s))
- Skip links: (add author(s))
- Interactive Areas: (add author(s))
- Focus: (add author(s))
- Mixed input: (add author(s))
- Keyboard shortcuts: (add author(s))
- Additional authors: (add author(s))

## Review

For this review, participants select a test they would like to complete and apply it to as many areas or states of the interface as they want in the given time.

### General notes

This is the place for anything a reviewer thinks is important that doesn't belong below. This could be something out of scope of the review, something that will impact all other tests, or the like.

Notes:

### Content order

When accessed via keyboard, the content order is logical. ([WCAG 2.2 Focus order](https://www.w3.org/TR/WCAG22/#focus-order))

1. From the top of the page, press the Tab key repeatedly until reviewer reaches the end of content.
2. Reviewers will know it is the end because if they press Tab once more their keyboard focus will return to the browser.
3. If the reviewer cannot make it to the end of content, please take note of where the focus gets stuck.

Does the content order follow reviewer expectations based on reading the content?
Result:

Does the content order make sense for interacting with the content?
Result:

Are any major content areas missed when navigating via keyboard?
Result:

Are any interactive content areas missed when navigating via keyboard?
Result:

Other notes or recommendations:

### Areas to navigate

All areas of the tool can be accessed using keyboard navigation. ([WCAG 2.2 Keyboard](https://www.w3.org/TR/WCAG22/#keyboard))

1. Navigate via the Tab key major content areas
2. Use the arrow keys to navigate within major content areas.

| Area | Able to navigate to the area (yes/no/not applicable) | Able to navigate fully within the area (yes/no/not applicable) | Able to navigate out of the area (yes/no/not applicable) |
|---|---|---|---|
| Navigation 1 | a | b | c |
| Navigation 2 | d | e | f |
| Aside/related content | g | h | i |
| Main area | j | k | l |
| Main area section | m | n | o |
| Footer | p | q | r |

Other notes by area:

### Keyboard/tab traps

When navigating via keyboard, there are no areas where keyboard focus can enter but not exit. The focus never gets "trapped." ([WCAG 2.2 No keyboard trap](https://www.w3.org/TR/WCAG22/#no-keyboard-trap))

1. From the top of the page, press the Tab key repeatedly until reviewer reaches the end of content.
2. Reviewers will know it is the end because if they press Tab once more their keyboard focus will return to the browser.
3. If the reviewer cannot make it to the end of content, please take note of where the focus gets stuck. If the reviewer can make it to all content, please note.
4. Optional: complete steps 1–3 over any areas that may have been missed by the content order. Using the mouse to move focus to an area and trying to tab out may be helpful for these cases.

Keyboard/tab traps:
- tab trap 1
- tab trap 2

Other notes or recommendations:

### Skip links

When using keyboard navigation, there is a link to switch keyboard focus directly to the tool's main content and skip header navigation or repeated content. ([WCAG 2.2 Bypass Blocks](https://www.w3.org/TR/WCAG22/#bypass-blocks))

1. From the top of the page, press the Tab key. If you have already been interacting with the page, reviewer may need to reload page and then press Tab.
2. Once focus is on the skip link, press Space or Enter to activate it.  

Is there a skip link?
Result:

Is the skip link prompt visible?
Result:

What does the skip link prompt skip?
Result:

Where does the skip link prompt move user focus to?
Result:

Does the skip link behavior meet reviewer expectations?
Result:

Other notes or recommendations:

### Interactive Areas

All buttons, links, form fields, or similar interactive areas can be both accessed and activated using only the keyboard. ([WCAG 2.2 Keyboard](https://www.w3.org/TR/WCAG22/#keyboard))

1. Navigate via the Tab key to interactive areas. 
2. Activate interactive areas using the Enter or Spacebar key.

| Interactive area | Able to navigate to the area (yes/no/not applicable) | Able to input information (yes/no/not applicable) | Able to activate the area (yes/no/not applicable) |
|---|---|---|---|
| Button 1| a | b | c |
| Button 2| d | e | f |
| Button 3 | g | h | i |
| Link 1 | j | k | l |
| Link 2 | m | n | o |
| Form field 1 | p | q | r |
| Add table rows as needed! |  |  |  |
| |  |  |  |

Other notes by area:

### Focus

There is a visible focus state for all content. It appears by default when navigating via keyboard. ([WCAG 2.2 Focus visible](https://www.w3.org/TR/WCAG22/#focus-visible))

1. From the top of the page, press the Tab key repeatedly until reviewer reaches the end of content. 
2. If end of content cannot be reached, the reviewer may report on what they could interact with.
3. If the reviewer is comfortable, they may also use the browser inspector to select an area and toggle focus per area.

Is there visible focus styling? If so, please briefly describe it.
Result:

Is the focus styling consistent throughout?
Result:

Are there any areas without visible focus styling?
Result: 

Was the reviewer ever unclear about where their keyboard focus was during the review? If so, please note where or why.
Result:

Other notes or recommendations:

### Mixed input

It is possible to complete tasks while switching between input mechanisms, for example using a keyboard and mouse and touch screen. ([WCAG 2.2 Concurrent input mechanisms](https://www.w3.org/TR/WCAG22/#concurrent-input-mechanisms))

1. Locate an interactive area.
2. Complete the interaction using keyboard controls.
3. Complete the interaction using the mouse.
4. Complete the interaction using touch controls.
5. If the task has multiple steps, the reviewer can try using a different interaction for each step.
6. Repeat as needed across interactive areas.

#### Task name + region

Repeat this section as needed for each task or region the reviewer evaluates.

Does the task have multiple steps? If yes, please list them.
Result:

Can the task be completed with only keyboard controls?
Result:

Can the task be completed with only mouse controls?
Result:

Can the task be completed with only touch screen contorls?
Result:

### Keyboard shortcuts

Keyboard shortcuts--key combinations that initiate an action-- may not inhibit keyboard navigation. Keyboard shortcuts also need to be configurable. ([WCAG 2.2 Character key shortcuts](https://www.w3.org/TR/WCAG22/#character-key-shortcuts))

[List of shortcuts for this tool]().

1. Search for where keyboard shortcut settings may be edited.
2. Review list of keyboard shortcuts.
3. Choose a shortcut and answer the prompts.
4. Repeat as needed.

Can shortcuts be turned off?
Result:

Can shortcuts be configured (remapped to different keys than the default)?
Result:

Do any shortcuts conflict with browser or operating system controls?
Result:

Other notes or recommendations:

#### Shortcut name

Repeat this section as needed for each shortcut the reviewer evaluates.

Shortcut keys:

How many keys are needed?
Result: 

How close together are the keys?
Result:

Does the shortcut only activate when focus is on the related part of the interface?
Result:

Other notes or recommendations: