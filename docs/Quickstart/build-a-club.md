---
sidebar_position: 1
---

# ⛳Build a Club

:::note

In practice, those are not really HTML elements, but React JSX elements, which we'll cover next!

:::


## Quotes {#quotes}

Markdown quotes are beautifully styled:

```md
> Easy to maintain open source documentation websites.
>
> — Docusaurus
```

<BrowserWindow>

> Easy to maintain open source documentation websites.
>
> — Docusaurus

</BrowserWindow>

Add **Markdown or React** files to `src/pages` to create a **standalone page**:

- `src/pages/index.js` → `localhost:3000/`
- `src/pages/foo.md` → `localhost:3000/foo`
- `src/pages/foo/bar.js` → `localhost:3000/foo/bar`


```mdx-code-block
<BrowserWindow>

<h3>Details element example</h3>

<details>
  <summary>Toggle me!</summary>
  <div>
    <div>This is the detailed content</div>
    <br/>
    <details>
      <summary>
        Nested toggle! Some surprise inside...
      </summary>
      <div>
        😲😲😲😲😲
      </div>
    </details>
  </div>
</details>

</BrowserWindow>
```

:::tip RDR2
~~The work around is to change the system date to 2022.~~
:::