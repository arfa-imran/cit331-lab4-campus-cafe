# HTTP observations (Lab 4, Task 1)
 
| Question | My answer |
|----------|-----------|
| Request method for index.html | ... |
| Status code with Disable cache ticked | ... |
| Status code on a normal reload | ... |
| Status code for /nothing-here.html | ... |
| Value of the Content-Type response header | ... |
| Remote Address (IP and port) | ... |
| Protocol in the address bar (http or https) | ... |
 
## Why is this address http and not https?
... (two sentences)
## Selectors I used

| Selector kind | Example from my CSS |
|---|---|
| Element | `body` |
| Class | `.card` |
| ID | `#main` |
| Grouping (comma) | `h1, h2, h3` |
| Descendant (space) | `.site-footer p` |
| Child (>) | `form > fieldset` |
| Adjacent sibling (+) | `h1 + p` |
| Compound (no space, such as a.active) | `a.active` |
| Attribute | `a[href^="http"]` |
| Pseudo-class | `a:hover` |
| Pseudo-element | `.menu-group h2::before` |











## Bug log (Lab 4, Task 6)

| # | What was wrong (file and line) | Which tool showed it | My fix |
|---|---|---|---|
| 1 | `debug/bugs.html`: The stylesheet link pointed to `style.css`, but the file was named `bugs.css`. | Network tab | Changed the stylesheet path to `bugs.css`. |
| 2 | `debug/bugs.html`: The HTML element did not declare the page language. | Lighthouse and W3C validator | Added `lang="en"` to the HTML element. |
| 3 | `debug/bugs.html`: Navigation links were inside a generic `div` rather than a navigation landmark. | Accessibility tree | Replaced the `div` with a `nav` element and added an accessible label. |
| 4 | `debug/bugs.html`: The heading jumped from `h1` to `h4`. | Accessibility tree and Lighthouse | Changed the second heading to `h2`. |
| 5 | `debug/bugs.html`: The logo image did not have alternative text. | Lighthouse | Added descriptive alternative text using the `alt` attribute. |
| 6 | `debug/bugs.html`: The label used `for="mail"`, but the input ID was `email`. | Lighthouse and manual label test | Changed the label to `for="email"`. |
| 7 | `debug/bugs.css`: The button's text-colour property was written as `colour`, which CSS does not recognise. | Styles pane | Changed `colour` to `color`. |
| 8 | `debug/bugs.css`: The hover background declaration did not end with a semicolon, preventing the following declaration from working correctly. | Styles pane | Added the missing semicolon. |
| 9 | `debug/bugs.css`: The selector `.notes` did not match the paragraph's class, which was `note`. | Styles pane | Changed `.notes` to `.note`. |
| 10 | `debug/bugs.css`: The paragraph text colour had insufficient contrast against its white background. | Lighthouse | Changed the text colour to `#595959`. |