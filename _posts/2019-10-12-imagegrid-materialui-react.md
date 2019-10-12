---
layout: post
title: "Image Grid using Material UI in React"
date: 2019-10-12 00:00:00 +0530
background: "/img/posts/04.jpg"
---

A simple example of a scrollable image grid using Material UI in ReactJS. We had a requirement for a scrollable image grid which will load images lazily. We started with the [Grid List](https://material-ui.com/components/grid-list/) example provided in Material UI.

We added a few more capabilities

1. Load images lazily
2. On clicking the tile, bigger size image is displayed with download option.

- Image Grid ![Image Grid](/img/posts/ss_0.png)
- Expaned Image ![Expanded Image](/img/posts/ss_1.png)

We also used [React Infinite Scroller](https://github.com/CassetteRocks/react-infinite-scroller) which is a simple, lightweight infinite scroll package that supports both window and scrollable elements.

Complete code is checked in at [GitHub](https://github.com/manisuec/Sandbox).

You can play around with at [CodeSandbox](https://codesandbox.io/embed/imagegrid-lepk2)
