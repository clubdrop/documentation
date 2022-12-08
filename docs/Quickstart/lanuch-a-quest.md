---
sidebar_position: 3
---
import Link from '@docusaurus/Link';
import VersionedLink from '@site/src/components/VersionedLink';
import ArrowRight from '@site/static/icons/arrow_right.svg';

# 🎉 Lanuch a quest

Docusaurus creates a **page for each blog post**, but also a **blog index page**, a **tag system**, an **RSS** feed...

## Create your first Post

Create a file at `blog/2021-02-28-greetings.md`:

```md title="blog/2021-02-28-greetings.md"
---
slug: greetings
title: Greetings!
authors:
  - name: Joel Marcey
    title: Co-creator of Docusaurus 1
    url: https://github.com/JoelMarcey
    image_url: https://github.com/JoelMarcey.png
  - name: Sébastien Lorber
    title: Docusaurus maintainer
    url: https://sebastienlorber.com
    image_url: https://github.com/slorber.png
tags: [greetings]
---

Congratulations, you have made your first post!

Feel free to play around and edit this post as much you like.
```

A new blog post is now available at [http://localhost:3000/blog/greetings](http://localhost:3000/blog/greetings).

 <div className='sub-heading'>
    <h3>Popular Topics</h3>
  </div>
  <div className='card'>
    <h4>Basics</h4>
    <p>You can get up and running with Hasura in minutes by following our Getting Started guide.</p>
    <VersionedLink to='/Quickstart/build-a-club.md'>
      See Getting Started <ArrowRight className='arrow' />
    </VersionedLink>
  </div>
  <div className='card'>
    <h4>GraphQL API</h4>
    <p>We provide an instant GraphQL API by generating your GraphQL schema for you based on your data.</p>
    <VersionedLink to='/Quickstart/build-a-club.md'>
      See Schema <ArrowRight className='arrow' />
    </VersionedLink>
  </div>
