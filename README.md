# Applied Linguistics for Language Education

Open teaching resources for language teacher education, by Achilleas Kostoulas. Each resource is a self-contained web page that accompanies a post on [achilleaskostoulas.com](https://achilleaskostoulas.com).

## Structure

```
index.html                        landing page listing the resources
what-is-applied-linguistics/
  index.html                      the workbench for that post
every-language-is-someones-world/
  index.html                      self-study activities for that post
reflecting-in-action/
  index.html                      guided reflective cycle for the practicum
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

### Independent learning unit: Language, multilingualism and language policy

Self-study activities based on the post [Every Language Is Someone's World: Reflections on International Mother Language Day 2026](https://achilleaskostoulas.com/2026/02/23/international-mother-language-day-2/). Each activity has its own page, reached from a contents list in the sidebar:

- **Start here**: who the resource is for, how it works, a note for readers who are not from Greece, links to the post and to Kostoulas, and the licence.
- **Warm-up**: a word from home that does not translate.
- **Activities 1 and 2** (before reading): a list of the reader's own languages, and six statements to agree or disagree with.
- **Activities 3 to 8** (while reading): one per section of the post, covering first-language criteria, language and dialect, the monolingual myth, second and foreign languages and repertoires, the three dimensions of language policy, and deficit versus resource framings.
- **Activity 9** (after reading): the six statements revisited, and a short written response.
- **Closing reflection**, then a final page with a **self-assessment** checklist, **reading trails** to linked texts and a **reading log**.

Readers choose one of two routes on the opening page. The **core route** (approximately 60–90 minutes) covers Activities 2, 3, 4, 6, 7 and 9 and the self-assessment; the **full route** (approximately 3.5 hours) covers everything. The contents list and the Back and Next buttons follow the chosen route, which can be changed at any time without losing answers.

The resource is written for readers working without a tutor. Every activity ends with a collapsible self-check, Activity 6 checks its own answers, and earlier answers (the warm-up word, the language list, the six statements) reappear where later activities build on them. Boxes headed "If you are not from Greece" give visiting students, such as Erasmus students, a way into the Greek examples.

The sidebar also holds the name field and the export options: a Word document, a plain text file, or copy to clipboard. Because the set is meant to be done over several sittings, readers can also save a progress file (JSON) to their own device and load it later to refill every answer. The file is read in the browser and is not uploaded anywhere.

This resource is licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/).

### Reflecting in Action

A guided reflective cycle for student teachers on the teaching practicum, based on a modified version of the framework in Gibbs, G. (1988/2013). *Learning by doing: a guide to teaching and learning methods*. OSCLD. Students work through six stages for one lesson, activity or moment they taught:

1. **Description of action**
2. **Affective, behavioural and cognitive responses**
3. **Evaluation**
4. **Analysis**
5. **Conclusions**, including what the experience taught them about multilingual learners and learners with a migrant or refugee background
6. **Action plan**

The stages are drawn as a clickable wheel that shows which stages are complete. Each stage has its guiding questions, a tip where useful, and a collapsible set of *If… then* prompts for when the student is stuck or wants to go further. Several of these prompts steer away from deficit framings of learners and from grammar-only evidence of success.

Each student writes six numbered reflections over the practicum. The top of the page holds their name, semester and the reflection number. A review screen gathers the reflection, and the student exports it as a PDF headed with their name, semester, reflection number and date, or copies it as text.

The PDF is generated in the browser with [jsPDF](https://github.com/parallax/jsPDF), which is bundled into the page along with a subset of the DejaVu Sans font (Latin, Greek and Cyrillic). The page makes no external requests, so PDF export also works offline.

## Privacy

No page sends anything anywhere. There is no server, no database, no analytics and no cookies.

The first two resources also use no browser storage: answers exist only in the open tab and are lost on reload, which each page states clearly at the top. Participants keep their work by copying it or saving the PDF.

Reflecting in Action is the exception, because the six reflections are written over several weeks. It keeps drafts in the browser's local storage, on the participant's own device, and the page says so at the top. Drafts are lost if the participant clears their browser data or changes device, so the page also lets them save a progress file (JSON) and load it again later on any device. The file is read in the browser and is not uploaded anywhere.

The PDF is generated in the participant's own browser using [pdfmake](https://pdfmake.github.io/docs/), loaded from the jsDelivr CDN. That request carries nothing the participant has typed. If the library fails to load, the page says so and directs participants to the copy option instead. To remove the external request entirely, download `pdfmake.min.js` and `vfs_fonts.js` into the resource's folder and change the two `<script src>` tags in its `index.html` to point at the local copies.

The Word document in the independent learning unit is generated in the same way using [docx](https://docx.js.org/), also loaded from jsDelivr. If that library fails to load, the page saves a simpler Word-compatible file instead, so export still works offline.

## Hosting

- **GitHub Pages** — in Settings → Pages, set the source to the `main` branch, root folder. The collection is then at `https://aikostoulas.github.io/AL-LE/`.
- **Moodle, Blackboard or similar** — upload a resource's `index.html` as a file resource, or paste its contents into an HTML block.
- **WordPress** — upload the file to `/wp-content/uploads/` and link to it, or embed it in an iframe.
- **Offline** — open the file directly in a browser. Everything works except PDF export, which needs the CDN unless you bundle the library locally.

## Credit

Content adapted from posts by Achilleas Kostoulas at <https://achilleaskostoulas.com>, with each resource naming and linking its source post.

Brumfit's definition is quoted from Brumfit, C. J. (1995). Teacher professionalism and research. In G. Cook & B. Seidlhofer (eds.), *Principle and Practice in Applied Linguistics*. Oxford: Oxford University Press, p. 27.

© 2026 Achilleas Kostoulas | Applied Linguistics & Language Teacher Education
