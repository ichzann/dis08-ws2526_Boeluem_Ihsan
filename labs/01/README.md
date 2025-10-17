# Basic Formatting

# Headings:
Durch das Symbol `#` wird die Schrift größer (1 = ganz groß → 6 = kleiner).  
**Bspl:**
### H3
#### H4
##### H5
###### H6

---

# Paragraphs & line breaks:
Mit **einer Leerzeile** erzeugst du Absätze.  
Mit `<br>` (ohne Punkt/Leerzeichen) machst du einen Zeilenumbruch **im selben Absatz**.  
**Bspl:**  
This line is <br> split by the `<br>` tag.

---

# Bold:
Entweder durch `**Text**` oder `__Text__` kannst du Text **fett** formatieren.  
**Bspl:**  
This **word** is bold.  
This __word__ is bold.

---

# Italic:
Mit `*Text*` oder `_Text_` kannst du *kursiv* schreiben.  
**Bspl:**  
This *word* is italic.  
This _word_ is italic.

---

# Strikethrough:
Mit `~~Text~~` kannst du ~~durchstreichen~~ (GFM/CommonMark).  
**Bspl:**  
This is ~~old~~ new.

---

# Inline code:
Mit Backticks \`…\` markierst du Code im Fließtext.  
**Bspl:**  
Use `inline code` inside a sentence.  
``Use ``backticks`` safely``

---

# Lists

# Unordered lists:
Mit `-`, `*` oder `+` erstellst du Aufzählungen.  
**Bspl:**
- Punkt A  
- Punkt B  
  - Unterpunkt B1  
* Punkt C  
+ Punkt D

---

# Ordered lists:
Mit `1.`, `2.`, … erstellst du nummerierte Listen (Zahlen im Quelltext dürfen auch alle `1.` sein, Renderer zählt hoch).  
**Bspl:**
1. Schritt  
1. Schritt  
1. Schritt

---

# Nested lists:
Mit Leerzeichen einrücken (meist 2–4), um zu verschachteln.  
**Bspl:**
1. Eltern  
   1. Kind  
      - Enkel

---

# Links & Images

# Inline links:
`[Text](URL "optional title")`  
**Bspl:**  
Siehe den [Markdown-Tutorial](https://www.markdowntutorial.com/ "Great intro")

---

# Reference-style links:
Linkziele separat definieren, besser lesbar.  
**Bspl:**  
Lies die [Hilfe][help]. Nochmals [help].

[help]: https://commonmark.org/help/ "CommonMark Help"

---

# Images:
`![Alt-Text](URL "optional title")` — Alt-Text hilft bei Accessibility.  
**Bspl:**  
![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png "GitHub Octocat")

---

# Image + link combination:
Bild in einen Link einbetten.  
**Bspl:**  
[![Go to GitHub](https://github.githubassets.com/images/icons/emoji/octocat.png)](https://github.com/)

---

# Code & Technical Content

# Inline code:
Wie oben: \`code\` im Text.  
**Bspl:**  
Press `Ctrl+C` to copy.

---

# Fenced code blocks:
Drei Backticks oder Tilden für mehrzeilige Codeblöcke.  
**Bspl:**


# Quotes & Notes

# Blockquotes:
Mit `>` beginnend.  
**Bspl:**
> Das ist ein Zitat.

---

# Nested blockquotes:
Mit mehreren `>` Ebenen verschachteln.  
**Bspl:**
> Außen  
>> Innen

---

# Blockquotes mit Formatierung:
Im Zitat sind **Fett**, *Kursiv*, `Code` und Listen erlaubt.  
**Bspl:**
> **Hinweis:** *Kursiv*, `Code` und Liste:
> - eins
> - zwei

---

# Tables

# Basic tables:
Pipes `|` und Trennlinie mit `-`; Kopfzeile erforderlich.  
**Bspl:**
| Tier  | Laut |
|-----:|:----:|
| Hund | Woof |
| Cat  | Meow |

---

# Alignment:
Ausrichtung per Doppelpunkten in der Trennzeile: `:---` links, `:---:` zentriert, `---:` rechts.  
**Bspl:**
| Links | Mitte | Rechts |
|:------|:-----:|------:|
| a     |   b   |     c |

---

# Complex tables:
Row/Col-Span geht im puren Markdown nicht; verwende ggf. HTML (plattformabhängig).  
**Bspl (HTML):**
<table>
  <thead>
    <tr><th>Feature</th><th>Support</th></tr>
  </thead>
  <tbody>
    <tr><td>Row/Col span</td><td>Use HTML</td></tr>
  </tbody>
</table>

---

# Task Lists

# Checkboxes:
GitHub Flavored Markdown: `- [ ]` offen, `- [x]` erledigt (auf GitHub anklickbar).  
**Bspl:**
- [ ] Markdown lernen  
- [x] Cheatsheet schreiben

---

# Dividers & Layout

# Horizontal rules:
Drei oder mehr `---`, `***` oder `___` in eigener Zeile.  
**Bspl:**

Text oben

---

Text unten

---

# Line breaks:
Zwei Leerzeichen am Zeilenende **oder** `<br>` für Umbruch im selben Absatz.  
**Bspl:**  
Erste Zeile  
Zweite Zeile (durch zwei Leerzeichen am Ende der ersten)

---

# Online and collaborative editors

# Markdown-basierte Editoren:
Beispiele (Feature-Support variiert):  
- Typora, Obsidian, VS Code (Markdown Preview), Zettlr  
- StackEdit, HackMD, Notion (Import/Export), GitHub/GitLab Editor  
- Joplin, Dendron, Foam

---

# Platform/Tool Specific: GitHub

# Task lists:
**Bspl:**
- [ ] open an issue  
- [x] close an issue

---

# Mentioning users (@username):
**Bspl:**  
Danke, @octocat!

---

# Automatic linking of issues/PRs:
`#123` verlinkt auf Issue/PR im selben Repo.  
**Bspl:**  
Fixes #123 and relates to PR #456.

---

# Emoji shortcodes:
`:shortcode:` rendert Emojis (z. B. auf GitHub).  
**Bspl:**  
Ship it! :rocket: :tada:

---

# Wichtig
Lege diese Inhalte bei Bedarf als `cheatsheet.md` in deinem Repo ab und erweitere sie im Semester.
