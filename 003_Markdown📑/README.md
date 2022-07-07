# **MARKDOWN**

[Markdownguide.org](https://www.markdownguide.org/basic-syntax/ "Syntax")

[GitHub.com](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax "Syntax")

**`.md = markdown (Značkovací jazyk)`**

---

## **The Basic:**

- ### **6x HEADER**

  ```markdown
  # Header One

  ## Header Two

  ### Header Three

  #### Header Four

  ##### Header Five

  ###### Header Six
  ```

  🐍 **`Rendered Output:`**

  # Header One

  ## Header Two

  ### Header Three

  #### Header Four

  ##### Header Five

  ###### Header Six

  ***

- ### **PARAGRAPHS**

  ```markdown
  Frist Paragraphs.

  Second Paragraphs.
  ```

  🐍 **`Rendered Output:`**

  Frist Paragraphs.

  Second Paragraphs.

  ***

- ### **LINE BREAKS**

  ```markdown
  First line. <br>
  Next line.
  ```

  🐍 **`Rendered Output:`**

  First line. <br>
  Next line.

  ***

- ### **HORIZONTAL LINE**

  ```markdown
  ---
  ```

  🐍 **`Rendered Output:`**

  ***

---

## **Text Formatting:**

- ### **BOLD**

  ```markdown
  **Bold Text**
  ```

  🐍 **`Rendered Output:`**

  **Bold Text**

  ***

- ### **ITALIC**

  ```markdown
  _Italic Text_
  ```

  🐍 **`Rendered Output:`**

  _Italic Text_

  ***

- ### **ITALIC + BOLD**

  ```markdown
  **Bold Text** _Italic Text_
  ```

  🐍 **`Rendered Output:`**

  **Bold Text** _Italic Text_

  ***

- ### **All Bold and Italic**

  ```markdown
  **_Bold and Italic Text_**
  ```

  🐍 **`Rendered Output:`**

  **_Bold and Italic Text_**

  ***

- ### **Strike Through**

  ```markdown
  ~~Strike Through~~
  ```

  🐍 **`Rendered Output:`**

  ~~Strike Through~~

  ***

- ### **backtick**

  ```markdown
  `backtick`
  ```

  🐍 **`Rendered Output:`**

  `backtick`

  ***

- ### **Subscript**

  ```markdown
  <sub>Subscript</sub>
  ```

  🐍 **`Rendered Output:`**

  <sub>Subscript</sub>

  ***

- ### **Superscript**

  ```markdown
  <sup>Superscript</sup>
  ```

  🐍 **`Rendered Output:`**

  <sup>Superscript</sup>

---

## **BLOCKQUOTES:**

- ### **BLOCKQUOTES SYNTAX**

  ```markdown
  > Blockquotes Text
  ```

  🐍 **`Rendered Output:`**

  > Blockquotes Text

  ***

- ### **BLOCKQUOTES WITH MULTIPLE PARAGRAPHS**

  ```markdown
  > Frist Paragraphs.
  >
  > Second Paragraphs.
  ```

  🐍 **`Rendered Output:`**

  > Frist Paragraphs.
  >
  > Second Paragraphs.

  ***

- ### **NESTED BLOCKQUOTES**

  ```markdown
  > Blockquotes Text
  >
  > > Nested Blockquotes Text
  ```

  🐍 **`Rendered Output:`**

  > Blockquotes Text
  >
  > > Nested Blockquotes Text

  ***

- ### **BLOCKQUOTES WITH OTHER ELEMENTS**

  ```markdown
  > #### Header4
  >
  > - First item
  > - Second item
  >
  > _Italic Text_ **Bold Text**.
  ```

  🐍 **`Rendered Output:`**

  > #### Header4
  >
  > - First item
  > - Second item
  >
  > _Italic Text_ **Bold Text**.

---

## **LISTS:**

- ### **ORDERED LIST**

  ```markdown
  1. First item
  2. Second item
  3. Third item

     1. Indented item
     2. Indented item

     - Indented item

  4. Fourth item
  ```

  🐍 **`Rendered Output:`**

  1. First item
  2. Second item
  3. Third item
     1. Indented item
     2. Indented item
     - Indented item
  4. Fourth item

  ***

- ### **UNORDERED LIST**

  ```markdown
  - First item
  - Second item
  - Third item
    - Indented item
    - Indented item
    1. Indented item
  - Fourth item
  ```

  🐍 **`Rendered Output:`**

  - First item
  - Second item
  - Third item
    - Indented item
    - Indented item
    1. Indented item
  - Fourth item

  ***

- ### **STARTING UNORDERED LIST ITEMS WITH NUMBERS**

  **`Escape -> 1968\`**

  ```markdown
  - 1968\. A great year!
  - I think 1969 was second best.
  ```

  🐍 **`Rendered Output:`**

  - 1968\. A great year!
  - I think 1969 was second best.

---

## **CODE BLOCK**

- ### **CODE BLOCK SYNTAX**

  **`Syntax Highlighting -> js,json,md...`**

  https://support.codebasehq.com/articles/tips-tricks/syntax-highlighting-in-markdown

  ***

  \`\`\`js

  {

  "firstName": "Pika",

  "lastName": "Heim",

  "age": 33

  }

  \`\`\`

  🐍 **`Rendered Output:`**

  ```js
  {
    "firstName": "Pika",
    "lastName": "Heim",
    "age": 33
  }
  ```

  ***

  \`\`\`diff

  {

  -"firstName": "Pika",

  +"lastName": "Heim",

  "age": 33

  }

  \`\`\`

  🐍 **`Rendered Output:`**

  ```diff
  {

  -"firstName": "Pika",

  +"lastName": "Heim",

  "age": 33

  }
  ```

---

## **IMAGES:**

- ### **IMAGES SYNTAX**

  ```markdown
  ![Alternate te Image](./../001_Logo🐍/PikaHeim_591x443.jpg)
  ```

  🐍 **`Rendered Output:`**

  ![Alternate te Image](./../001_Logo🐍/PikaHeim_591x443.jpg)

  ***

- ### **TITLES**

  ```markdown
  ![Alternate te Image](./../001_Logo🐍/PikaHeim_591x443.jpg "Logo")
  ```

  🐍 **`Rendered Output:`**

  ![Alternate te Image](./../001_Logo🐍/PikaHeim_591x443.jpg "Logo")

  ***

- ### **Transparent PNG images**

  **`Dle motivu prohlížeče (Tmavý/Světlý)`**

  **`HTM element`**

  ```markdown
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/25423296/163456776-7f95b81a-f1ed-45f7-b7ab-8fa810d529fa.png">
    <source media="(prefers-color-scheme: light)" srcset="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
    <img alt="Shows an illustrated sun in light color mode and a moon with stars in dark color mode." src="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
  </picture>
  ```

  🐍 **`Rendered Output:`**

   <picture>
     <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/25423296/163456776-7f95b81a-f1ed-45f7-b7ab-8fa810d529fa.png">
     <source media="(prefers-color-scheme: light)" srcset="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
     <img alt="Shows an illustrated sun in light color mode and a moon with stars in dark color mode." src="https://user-images.githubusercontent.com/25423296/163456779-a8556205-d0a5-45e2-ac17-42d089e3c3f8.png">
   </picture>

---

## **LINKS:**

- ### **LINKS SYNTAX**

  ```markdown
  [Markdownguide.org](https://www.markdownguide.org/)
  ```

  🐍 **`Rendered Output:`**

  [Markdownguide.org](https://www.markdownguide.org/)

  ***

- ### **TITLES**

  ```markdown
  [Markdownguide.org](https://duckduckgo.com "Titles")
  ```

  🐍 **`Rendered Output:`**

  [Markdownguide.org](https://duckduckgo.com "Titles")

  ***

- ### **URL and EMAIL ADRESSES**

  ```markdown
  <https://www.markdownguide.org>
  <fake@example.com>
  ```

  🐍 **`Rendered Output:`**

  <https://www.markdownguide.org>

  <fake@example.com>

---

## **ESCAPING CHARACTERS**

**`\ + Character`**

| Character | Name                |
| :-------- | :------------------ |
| \\        | Backslash           |
| \`        | Backtick            |
| \*        | Asterisk            |
| \_        | Underscore          |
| \{ \}     | Curly Braces        |
| \[ \]     | Brackets            |
| \< \>     | Angle Brackets      |
| \( \)     | Parentheses         |
| \#        | Pound Sign          |
| \+        | Plus Sign           |
| \-        | Minus Sign (Hyphen) |
| \.        | Dot                 |
| \!        | Exclamation Mark    |
| \|        | Pipe                |

### **Example🐲:**

```markdown
\{ \}
```

🐍 **`Rendered Output:`**

\{ \}

---

## **TABLES**

```markdown
| Header0   | Header1  |    Header2 | Header3 |
| :-------- | :------: | ---------: | ------- |
| TextLeft  | TextMid  |  TextRight | Text    |
| TextLeft1 | TextMid1 | TextRight1 | Text1   |
```

🐍 **`Rendered Output:`**

| Header0   | Header1  |    Header2 | Header3 |
| :-------- | :------: | ---------: | ------- |
| TextLeft  | TextMid  |  TextRight | Text    |
| TextLeft1 | TextMid1 | TextRight1 | Text1   |

---
