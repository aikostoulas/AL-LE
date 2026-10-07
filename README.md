# Applied Linguistics for Language Education

Open teaching resources for language teacher education, by Achilleas Kostoulas. Each resource is a self-contained web page that accompanies a post on [achilleaskostoulas.com](https://achilleaskostoulas.com).

## Structure

```
index.html                        landing page listing the resources
what-is-applied-linguistics/
  index.html                      the workbench for that post
every-language-is-someones-world/
  index.html                      self-study activities for that post
```

Each resource lives in its own folder with an `index.html` inside it, so it is served at a clean address such as `/AL-LE/what-is-applied-linguistics/` and can carry its own images or local copies of libraries without colliding with anything else. To add a resource, create a folder, put its `index.html` inside, and add an `<article>` block to the root `index.html`.

There is no build step and no framework. Every page is plain HTML, CSS and JavaScript in one file.

## Resources

### What is applied linguistics?

Six activities based on the post [What is applied linguistics?](https://achilleaskostoulas.com/2018/05/10/what-is-applied-linguistics/). They ask participants to produce something rather than recognise a correct answer:

1. **Rewrite the definition** — revise Brumfit's definition and test it against the four elements of the post.
2. **Where is the boundary?** — place six studies on a scale from general education to applied linguistics and justify each placement.
3. **So what? Now what?** — appraise a current method, app or coursebook by asking what view of language and learning it assumes.
4. **Answer a lay theory** — write a reply to a parent, colleague or policymaker who holds one of the lay beliefs discussed in the post.
5. **Challenge a given** — design a small, resource-light study to test an assumption held in your own school.
6. **Do teachers need theory?** — argue one side of the Medgyes debate, then name what you concede.

A final tab gathers everything the participant has written, which they can copy as text or save as a PDF.

The resource is designed for individual preparation before a shared discussion, not as a replacement for one. Activities 2 and 6 in particular are built to produce disagreement, and that disagreement has to happen somewhere else: a seminar, a forum, a shared document. Asking participants to post their copied text into a course forum is the simplest way to make that happen.

### Every Language Is Someone's World

Self-study activities based on the post [Every Language Is Someone's World: Reflections on International Mother Language Day 2026](https://achilleaskostoulas.com/2026/02/23/international-mother-language-day-2/). Each activity has its own page, reached from a contents list in the sidebar:

- **Start here**: who the resource is for, how it works, a note for readers who are not from Greece, links to the post and to Kostoulas, and the licence.
- **Warm-up**: a word from home that does not translate.
- **Activities 1 and 2** (before reading): a list of the reader's own languages, and six statements to agree or disagree with.
- **Activities 3 to 8** (while reading): one per section of the post, covering first-language criteria, language and dialect, the monolingual myth, second and foreign languages and repertoires, the three dimensions of language policy, and deficit versus resource framings.
- **Activity 9** (after reading): the six statements revisited, and a short written response.
- **Closing reflection**, then a final page with a **self-assessment** checklist, **reading trails** to linked texts and a **reading log**.

The resource is written for readers working without a tutor. Every activity ends with a collapsible self-check, Activity 6 checks its own answers, and earlier answers (the warm-up word, the language list, the six statements) reappear where later activities build on them. Boxes headed "If you are not from Greece" give visiting students, such as Erasmus students, a way into the Greek examples.

The sidebar also holds the name field and the export options: a Word document, a plain text file, or copy to clipboard. Because the set is meant to be done over several sittings, readers can also save a progress file (JSON) to their own device and load it later to refill every answer. The file is read in the browser and is not uploaded anywhere.

This resource is licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/).

## Privacy

The pages store nothing. There is no server, no database, no analytics, no cookies and no browser storage. Answers exist only in the open tab and are lost on reload, which the page states clearly at the top. Participants keep their work by copying it or saving the PDF.

The PDF is generated in the participant's own browser using [pdfmake](https://pdfmake.github.io/docs/), loaded from the jsDelivr CDN. That request carries nothing the participant has typed. If the library fails to load, the page says so and directs participants to the copy option instead. To remove the external request entirely, download `pdfmake.min.js` and `vfs_fonts.js` into the resource's folder and change the two `<script src>` tags in its `index.html` to point at the local copies.

The Word document in *Every Language Is Someone's World* is generated in the same way using [docx](https://docx.js.org/), also loaded from jsDelivr. If that library fails to load, the page saves a simpler Word-compatible file instead, so export still works offline.

## Hosting

- **GitHub Pages** — in Settings → Pages, set the source to the `main` branch, root folder. The collection is then at `https://aikostoulas.github.io/AL-LE/`.
- **Moodle, Blackboard or similar** — upload a resource's `index.html` as a file resource, or paste its contents into an HTML block.
- **WordPress** — upload the file to `/wp-content/uploads/` and link to it, or embed it in an iframe.
- **Offline** — open the file directly in a browser. Everything works except PDF export, which needs the CDN unless you bundle the library locally.

## Credit

Content adapted from posts by Achilleas Kostoulas at <https://achilleaskostoulas.com>, with each resource naming and linking its source post.

Brumfit's definition is quoted from Brumfit, C. J. (1995). Teacher professionalism and research. In G. Cook & B. Seidlhofer (eds.), *Principle and Practice in Applied Linguistics*. Oxford: Oxford University Press, p. 27.

© 2026 Achilleas Kostoulas | Applied Linguistics & Language Teacher Education
