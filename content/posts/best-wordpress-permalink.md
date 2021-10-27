---
title: Best Permalink Structure for WordPress
description: After years of experience, this is what I come down to for permalink structure in WordPress.
date: 2021-10-27T23:24:56+05:30
tags: [tech, blogging]
---

I've tried `compile.blog/new-post/`, `compile.blog/posts/new-post/`, `compile.blog/2021/10/new-post/`, etc. permalinks for my WordPress blogs.

But... now, I think I've found the perfect permalink structure, and that'd be:

`compile.blog/{category}/new-post/`

Yes, `{category}` here is a variable. For example, if I published a new post in the `business` category, then the post URL would be:

`compile.blog/business/new-post/`

And, then I'd 301 redirect the individual **category page** to a new custom page where all the posts from that category will be show with some extra information. See below:

`compile.blog/category/business/` will be 301 redirected to `compile.blog/business/` and then post's permalink structure in this category is already `compile.blog/business/{new-post}/`

But why? Why would I do that?

Well, the default category pages can't be customized enough. You cannot add much information on the page. But when all the category pages are redirected to their respective pages, those are better for adding extra information.

This setup is also helpful to create relevant topic clusters for better search engine rankings.

Currently, I haven't applied it anywhere but I think it'll work, for sure.
