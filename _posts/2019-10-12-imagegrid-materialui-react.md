---
layout: post
title: "Image Grid using Material UI in React"
date: 2019-10-12 00:00:00 +0530
background: "/img/posts/04.jpg"
---

A simple example of a scrollable image grid using Material UI in ReactJS. We had a requirement for a scrollable image grid which will load images lazily. We started with the [Grid List](https://material-ui.com/components/grid-list/) example provided in Material UI.

We added a few more capabilities

- Load images lazily
- On clicking the tile, bigger size image is displayed with download option.

Few screenshots of the image grid

1. Image Grid ![Image Grid](/img/posts/ss_0.png)
2. Expaned Image ![Expanded Image](/img/posts/ss_1.png)

We also used [React Infinite Scroller](https://github.com/CassetteRocks/react-infinite-scroller) which is a simple, lightweight infinite scroll package that supports both window and scrollable elements.

The image metadata array provided is hardcoded in the example code. This can be passed to the imagegrid component as a prop and fetched from your application's api endpoint. We store the metadata in our database and actual images in different resolutions are stored in Amazon S3.

Complete code is checked in at [GitHub](https://github.com/manisuec/Sandbox).

You can play around with at [CodeSandbox](https://codesandbox.io/embed/imagegrid-lepk2)
