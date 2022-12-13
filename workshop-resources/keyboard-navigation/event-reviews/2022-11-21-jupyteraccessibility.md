# Collaborative keyboard navigation review

Please add your findings as [GitHub suggestions](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/commenting-on-a-pull-request) so you are credited in the commit history!

## Keyboard navigation accessibility review of [Jupyter accessibility documentation](https://jupyter-accessibility.readthedocs.io/en/latest/index.html)

Reviewed via browser based on [this link we'll all be working off of](https://jupyter-accessibility.readthedocs.io/en/latest/index.html).

- Review date: 21 November 2022
- Operating system:
- Browser: 
- Keyboard language(s) used:
- Any other details (ie. dependencies, github repo, etc.):

### Authors and contents

- Content order: @trallard
- ~~Areas to navigate:~~ Not completed
- ~~Keyboard/tab traps:~~ Not completed
- Skip links: @trallard
- Interactive Areas: @gabalafou
- ~~Focus:~~ Not completed
- Mixed input: @isabela-pf 
- ~~Keyboard shortcuts:~~ Not completed

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
