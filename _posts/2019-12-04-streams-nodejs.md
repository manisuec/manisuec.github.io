---
layout: post
title: "Streams: An underrated but very powerful concept in NodeJS"
date: 2019-12-04 00:00:00 +0530
background: "/img/posts/04.jpg"
---

A stream is an abstract interface for working with streaming data in Node.js. Streams have gained the reputation that it is hard to work with and harder to understand. However, it is a highly underrated but very powerful concept in Node.js. This article will help in understanding of streams, how to work with them and where to use this module.

## Streams: Introduction


The official documentation of Node.js defines stream as an abstract interface for working with streaming data. It is one of the fundamental concept in Node.js  and is very powerful when working with large amounts of data, e.g., reading a very large file size. Streams are memory efficient as there is no need to load large amount of data in memory instead read chunks of data piece by piece and process the contents. Also, since one doesn't have to wait for all the data to load first, it is time efficient too.

For a complete introduction of Stream module and its related apis, read the [official documentation.](!https://nodejs.org/dist/latest-v12.x/docs/api/stream.html)

## Streams: A use case

For the purpose of showing the powerful capability of streams, let us do the following operations.

1. Read data from a large file.
2. Filter the data.
3. Transform the input data.
4. Write the transformed data into a file.

I have downloaded the [Loan Data for Dummy Bank](!https://www.kaggle.com/mrferozi/loan-data-for-dummy-bank/data) file for this article. Let us read the data from the file, filter out all those who have 'RENT' as value for home_owner column. Then mark the filtered out rows having loan amount to annual income ratio as > 10% as high credit risk else low credit risk and write into a new file.


