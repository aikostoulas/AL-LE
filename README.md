# What is applied linguistics? A workbench for language teachers

Six online activities for language teacher education, based on the blog post
[What is applied linguistics?](https://achilleaskostoulas.com/2018/05/10/what-is-applied-linguistics/)
by Achilleas Kostoulas.

The activities ask participants to produce something rather than recognise a correct answer:

1. **Rewrite the definition** — revise Brumfit's definition and test it against the four elements of the post.
2. **Where is the boundary?** — place six studies on a scale from general education to applied linguistics and justify each placement.
3. **So what? Now what?** — appraise a current method, app or coursebook by asking what view of language and learning it assumes.
4. **Answer a lay theory** — write a reply to a parent, colleague or policymaker who holds one of the lay beliefs discussed in the post.
5. **Challenge a given** — design a small, resource-light study to test an assumption held in your own school.
6. **Do teachers need theory?** — argue one side of the Medgyes debate, then name what you concede.

A final tab gathers everything the participant has written, which they can copy as text or save as a PDF.

## Privacy

The page stores nothing. There is no server, no database, no analytics, no cookies and no browser storage. Answers exist only in the open tab and are lost on reload, which the page states clearly at the top. Participants keep their work by copying it or saving the PDF.

The PDF is generated in the participant's own browser using [pdfmake](https://pdfmake.github.io/docs/), loaded from the jsDelivr CDN. That request carries nothing the participant has typed. If the library fails to load, the page says so and directs participants to the copy option instead. To remove the external request entirely, download `pdfmake.min.js` and `vfs_fonts.js` into this repository and change the two `<script src>` tags in `index.html` to point at the local copies.

## Using it

The whole resource is the single file `index.html`. There is no build step.

- **GitHub Pages** — in Settings → Pages, set the source to the `main` branch, root folder.
- **Moodle, Blackboard or similar** — upload `index.html` as a file resource, or paste its contents into an HTML block.
- **WordPress** — upload the file to `/wp-content/uploads/` and link to it, or embed it in an iframe.
- **Offline** — open the file directly in a browser. Everything works except PDF export, which needs the CDN unless you bundle the library locally.

## Teaching notes

The resource is designed for individual preparation before a shared discussion, not as a replacement for one. Activities 2 and 6 in particular are built to produce disagreement, and that disagreement has to happen somewhere else: a seminar, a forum, a shared document. Asking participants to post their copied text into a course forum is the simplest way to make that happen.

## Credit

Content adapted from Achilleas Kostoulas, *What is applied linguistics?*, published 10 May 2018 and revised since, at
<https://achilleaskostoulas.com/2018/05/10/what-is-applied-linguistics/>.

Brumfit's definition is quoted from Brumfit, C. J. (1995). Teacher professionalism and research. In G. Cook & B. Seidlhofer (eds.), *Principle and Practice in Applied Linguistics*. Oxford: Oxford University Press, p. 27.

© 2026 Achilleas Kostoulas | Applied Linguistics & Language Teacher Education
