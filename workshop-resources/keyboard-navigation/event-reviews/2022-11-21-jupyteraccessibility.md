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
- Skip links: (add author(s)) @trallard
- Interactive Areas: @gabalafou
- Focus: (add author(s))
- Mixed input: @isabela-pf 
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

Kind of - the order is as follows:

1. Left sidebar: logo -> search bar -> sidebar items (top to down)
1. Top left menu: icons left to right
1. Table of contents: TOC items top to bottom
1. Main content: links as they appear top to bottom -> Next navigation button

I would expect Areas to go left to right in a left-to-right language
At no given point I accessed the footer

Does the content order make sense for interacting with the content?
Result:

I suppose it does - even if I find it confusing with the jumps left -> right -> center

Are any major content areas missed when navigating via keyboard?
Result:

There is no way to access the left sidebar footer (versions) or the hamburger menu (collapse sidebar)

Are any interactive content areas missed when navigating via keyboard?
Result:

- There is no way to access the dropdown menus in the left-sidebar
- Cannot access the hamburger menu (which should be a collapse icon instead)

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
No there is not

Is the skip link prompt visible?
Result:

N/A

What does the skip link prompt skip?
Result:

N/A

Where does the skip link prompt move user focus to?
Result:

N/A

Does the skip link behavior meet reviewer expectations?
Result:

I hoped there would be a skip link

Other notes or recommendations:

Would suggest adding a skip link that would redirect the reader to the main content area

### Interactive Areas

All buttons, links, form fields, or similar interactive areas can be both accessed and activated using only the keyboard. ([WCAG 2.2 Keyboard](https://www.w3.org/TR/WCAG22/#keyboard))

1. Navigate via the Tab key to interactive areas. 
2. Activate interactive areas using the Enter or Spacebar key.

| Interactive area | Able to navigate to the area (yes/no/not applicable) | Able to input information (yes/no/not applicable) | Able to activate the area (yes/no/not applicable) |
|---|---|---|---|
| Fullscreen mode button | yes | n/a | yes (pressing Enter or Space key turns on/off fullscreen mode) |
| GitHub icon dropdown | no | n/a | no (but if I open the dropdown with a mouse click, then I can activate the dropdown options with keyboard) |
| Download icon dropdown | no | n/a | no (but if I open the dropdown with a mouse click, then I can activate the dropdown options with keyboard) |
| Toggle navigation button ("hamburger" / triple line) | no | no | no |
| Read the Docs version switcher | no | no | no |
| Links in left side nav (Jupyter accessibility logo link to Jupyter Book link) | yes | n/a | yes (pressing Enter key opens the link) |
| Links in main area (from "Classic Jupyter Notebook" to "Next Jupyter Accessibility Statement") | yes | n/a | yes (pressing Enter key opens the link) |
| The two links in the right side nav | yes | n/a | yes (ditto) |
| Search this book... | yes | yes | yes (pressing Enter after typing search term performs a search on the docs) |
| Collapse/expand button in left nav | no | n/a | no |

Other notes by area:
- Left side nav:
    - While the collapse/expand buttons in the left side nav cannot be accessed (and therefore can be activated using only the keyboard), the link adjacent to each expand button can be opened using the keyboard, which as the effect (after a round trip to the server) of opening/expanding that section in the side nav. But the expand/collapse button should be usable with only a keyboard.
    - The search field has an clear "X" button that appears when you start typing characters in the search field. That X button is not reachable via keyboard; however, I'm not sure it's really needed... at least if you know that you can type ctrl+a followed by the delete key in order to quickly delete everything you typed into the the field.

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

#### Page drop down menus (ie. GitHub and Download icons)

Does the task have multiple steps? If yes, please list them.
Result: Tab to focus the page menu (GitHub and Download icons), reach focus for a menu with a drop down available, press space or enter, drop down menu appears, navigate drop down menu, select drop down item.

Can the task be completed with only keyboard controls?
Result: No. The menus can be tabbed to, but they cannot be activated to open the drop down with the keyboard. They can be activated and navigated with a mouse. Even if the menus are opened with a mouse, the user cannot switch to navigate them with a keyboard.

I was also surprised because the left and right arrow keys—typically used for fine-grain navigation through things like drop down menu items—immediately move me to the next page in the documentation. I am guessing this is because Jupyter Book is modeled like a book where turning pages to continue reading is high priority. The fact that it overrides keyboard navigation, concurrent with other navigation methods or not, is a problem.

Can the task be completed with only mouse controls?
Result: Yes.

Can the task be completed with only touch screen controls?
Result: n/a

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