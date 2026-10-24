# editedpiece

Two final HTML/CSS reference pages for Alexander Grubb's Web 1 project.

- **index.html:** bento-style panels, with history and examples from comics, manga, and manhwa.
- **collage.html:** collage history, instructions, and zine, punk, and scrapbook examples.
- **css/styles.css:** one shared stylesheet.
- **images/:** only the seven local images used by the final pages.

## Open the pages

Download the repository ZIP, extract it, and open the folder in VS Code. Open index.html in a browser, then use the navigation to visit Collage. Keep the css and images folders beside the HTML files. There is no JavaScript, framework, package installation, or build command.

The bento history illustration loads from Wikimedia Commons, so that image needs an internet connection. Its source link is at the bottom of the bento page. Other images are saved locally.

## How the code works

1. **Set up the files.** Make two HTML files and one CSS file. Put images in an images folder. Relative paths such as css/styles.css tell the browser where the files are.
2. **Write the HTML skeleton.** Use a doctype, html lang="en", head, and body. The head contains the title, character encoding, viewport setting, and stylesheet link.
3. **Add navigation.** Put ordinary a links in a list inside nav. index.html and collage.html link to each other. Links such as #history point to an element with id="history" on the same page.
4. **Build the page structure.** Use header for the hero, main for the content, section for each main topic, and footer for the closing navigation. HTML describes the content before CSS changes its appearance.
5. **Choose headings.** Use one h1 for the page title, h2 for the main sections, and h3 for smaller topics. Heading level follows importance, rather than just the font size.
6. **Add text and images.** Use p for paragraphs and img for pictures. Set src to the image path and write useful alt text. Put a caption in a p with class="image-caption" below its image. Research and image credits are collected at the bottom of each page.
7. **Connect classes to CSS.** class="card" in HTML matches .card in CSS. A body class such as bento-page lets the stylesheet give one page its own colors without changing the other.
8. **Set the basic appearance.** Start with fonts, colors, spacing, and readable line heights. :root holds repeated values as custom properties. For example, var(--space-medium) reuses the same spacing value.
9. **Arrange the layout.** Flexbox keeps navigation and footer links in rows. CSS Grid creates equal columns for the hero, examples, and collage history/how-to. The bento demonstration has four tracks; span 2 makes its main panel use two columns or rows.
10. **Add the visual details.** The comic page uses thick borders and yellow panels. The collage page uses straight paper-like blocks and different card colors. The images stay unobstructed and the text sits below them.
11. **Handle narrow screens.** A media query at 760px changes the main grids to one column. Grid spans are reset so the bento panels can stack.
12. **Check and save progress.** Test links, image paths, heading order, keyboard focus, and the narrow layout. Commit after a real change with a message describing what changed. A commit saves a version; pushing sends it to GitHub. Publishing through Vercel is a separate step.

## Familiar HTML elements

The HTML uses only elements found in the earlier practice repositories. header introduces a page or section, section groups a topic with a heading, article holds a complete example or history explanation, and aside holds a supporting image. span marks a title or step label within a line of text. div remains only around layout groups such as rows of cards and the footer contents.

These patterns can be compared with [practice 3](https://github.com/AlexGrubbMcc/practice-3-AlexGrubbMcc), [practice 4](https://github.com/AlexGrubbMcc/practice-4-AlexxGrubbMcc), and [practice 7](https://github.com/AlexGrubbMcc/practice-7-alexandergrubb).

## Image credits

The images are educational design references, not original student artwork. Copyrighted artwork and photographs belong to their creators and rights holders.

| Image | Source / credit |
| --- | --- |
| spider-man.png | [Marvel: Amazing Fantasy #15](https://www.marvel.com/comics/issue/16926), official website screenshot, © Marvel. Issue credits: Stan Lee, writer; Steve Ditko, penciller. |
| one-piece.png | [VIZ: One Piece](https://www.viz.com/one-piece), promotional website screenshot; Eiichiro Oda / Shueisha. |
| omniscient-reader.png | [WEBTOON: Omniscient Reader](https://www.webtoons.com/en/action/omniscient-reader/list?title_no=2154), website screenshot; singNsong, UMI, Sleepy-C. |
| studio-loop.png | [Studio Loop](https://www.studioloop.com.br/), website screenshot; site and artwork belong to their creators. |
| flipside.jpg | [University of Maryland Libraries](https://lib.guides.umd.edu/c.php?g=1378775&p=10803201), Flipside issue 51, Winter 1986; original photography and artwork belong to their rights holders. |
| personal-zines.jpg | [Norwich University of the Arts Library](https://library.norwichuni.ac.uk/guides/zines/), library photograph; individual covers belong to their creators. |
| mat.png | [Mat / Rahul Bhadoriya](https://www.matwidget.com/), website screenshot. |
| External history illustration | [Vieuxbois1.jpg on Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Vieuxbois1.jpg), Rodolphe Töpffer, 1837, public domain. The source scan is small, so enlarged lines may look soft. |

Research links for the written content are in each page's Sources and image credits section.

## Reference and assistance

This is a cleaned final snapshot copied from [project-one-AlexGrubbMcc](https://github.com/AlexGrubbMcc/project-one-AlexGrubbMcc). Earlier development commits remain in that original repository; they were not recreated here. Unused images and obsolete CSS rules are omitted.

ChatGPT assisted with the reference code, research, revisions, and checks. The student plans to study the code and rebuild it independently. Follow the teacher's rules for the submitted version; the assignment prohibits AI building the submitted pages.
