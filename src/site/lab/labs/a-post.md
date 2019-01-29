---
title: A lab page
date: 2019-01-23T19:00:00-05:00
---

There's not much here in the sample post page. Better get to work.

The common front-matter data for all of the files in the posts section are abstracted into a `labs.json` file so that we don't need to repeat that on every file. Handy.

It looks like this:

```
{
  "layout" : "layouts/lab.md",
  "tags" : "lab",
  "templateEngineOverride": "njk,md"
}
```


