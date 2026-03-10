---
layout: post
title: "Style Test: Everything You Can Put in a Post"
date: 2026-03-10 12:00:00 +0500
---

This is a normal paragraph. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Keep writing and the text just wraps naturally to the next line.

## Heading 2

This is text under a second-level heading. Use `##` for main sections.

### Heading 3

This is text under a third-level heading. Use `###` for subsections.

---

## Lists

An unordered list:

- First item
- Second item
- Third item with a bit more text to see how wrapping looks in list items

An ordered list:

1. Step one
2. Step two
3. Step three

Nested list:

- Parent item
  - Child item
  - Another child
- Back to parent

---

## Code

Inline code: use backticks to write `variableName` or `git commit -m "message"` inside a sentence.

A code block with syntax:

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, world!");
    }
}
```

```sql
SELECT u.name, COUNT(c.id) AS commits
FROM users u
JOIN commits c ON c.user_id = u.id
GROUP BY u.name
ORDER BY commits DESC;
```

```bash
./mvnw clean package -DskipTests
docker build -t pandev-metrics .
```

---

## Blockquote

> The purpose of abstracting is not to be vague, but to create a new semantic level in which one can be absolutely precise.
>
> — Edsger Dijkstra

---

## Links

A regular link: [GitHub](https://github.com/theberdakh)

A link inside a sentence: I published an open-source library called [From2](https://github.com/theberdakh/From2) for Karakalpak translation.

---

## Bold and Italic

**Bold text** is written with double asterisks.

*Italic text* is written with single asterisks.

**Bold and *italic* together** works too.

---

## Table

| Tool          | Purpose              | Used in         |
|---------------|----------------------|-----------------|
| Spring Boot   | Backend framework    | PanDev Metrics  |
| Testcontainers| Integration testing  | PanDev Metrics  |
| JGit          | Git operations       | PanDev Metrics  |
| Retrofit      | HTTP client          | Android apps    |

---

## Horizontal Rule

Three dashes make a divider like the ones above.

---

## Image

A basic image with alt text:

![A placeholder image](https://placehold.co/660x400)

Image with a caption (just italic text below it — Markdown has no native caption):

![Spring Boot module structure](https://placehold.co/660x300)
*Module dependency graph for a 20-module Maven project.*

Small inline-sized image:

![small](https://placehold.co/200x200)

---

## GIF

GIFs use the exact same syntax as images — the browser plays them automatically:

![Demo animation](https://media.giphy.com/media/xT9IgzoKnwFNmISR8I/giphy.gif)

To use your own GIF, put the file in `assets/` and reference it:

```markdown
![My demo]({{ '/assets/demo.gif' | relative_url }})
```

---

## PDF Embed

Embed a PDF inline using an `<iframe>`:

<iframe src="{{ '/assets/Berdakh_Tlepov_CV.pdf' | relative_url }}" width="100%" height="600px" style="border: 1px solid #e8e6e0; border-radius: 4px;"></iframe>

Or just link to it for download:

[Download CV (PDF)]({{ '/assets/Berdakh_Tlepov_CV.pdf' | relative_url }})

---

## YouTube Video

Embed a YouTube video using an `<iframe>`:

<iframe width="100%" height="380" src="https://www.youtube.com/embed/dQw4w9WgXcQ" frameborder="0" allowfullscreen style="border-radius: 4px;"></iframe>

---

## Image from your assets folder

Once you add an image to `assets/images/`, reference it like this:

```markdown
![My screenshot]({{ '/assets/images/screenshot.png' | relative_url }})
```

---

That's everything. Remove what you don't need in real posts.
