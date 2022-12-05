---
sidebar_position: 2
---

# 🎨Deploy/import contracts

start creative

Documents are **groups of pages** connected through:

- a **sidebar**
- **previous/next navigation**
- **versioning**

## Create your first Doc

Create a Markdown file at `docs/hello.md`:

```md title="docs/hello.md"
# Hello

This is my **first Docusaurus document**!
```

A new document is now available at [http://localhost:3000/docs/hello](http://localhost:3000/docs/hello).

## Configure the Sidebar

Docusaurus automatically **creates a sidebar** from the `docs` folder.

Add metadata to customize the sidebar label and position:

```md title="docs/hello.md" {1-4}
---
sidebar_label: 'Hi!'
sidebar_position: 3
---

# Hello

This is my **first Docusaurus document**!
```

It is also possible to create your sidebar explicitly in `sidebars.js`:

```js title="sidebars.js"
module.exports = {
  tutorialSidebar: [
    {
      type: 'category',
      label: 'Tutorial',
      // highlight-next-line
      items: ['hello'],
    },
  ],
};
```

<details>
  <summary>How are <code>remark-math</code> and <code>rehype-katex</code> different?</summary>

In case you are wondering how Remark and Rehype are different, here is a good example. `remark-math` operates on the Markdown AST, where it sees text like `$...$`, and all it does is transform that to the JSX `<span class="math math-inline">...</span>` without doing too much with the content. This decouples the extraction of math formulae from their rendering, which means you can swap $\KaTeX$ out with other math renderers, like MathJax (with [`rehype-mathjax`](https://github.com/remarkjs/remark-math/tree/main/packages/rehype-mathjax)), just by replacing the Rehype plugin.

Next, the `rehype-katex` operates on the Hypertext AST where everything has been converted to HTML-like tags already. It traverses all the elements with `math` class and uses $\KaTeX$ to parse and render the content to actual HTML.

</details>
