---
title: "Specifing package versions in package.json file"
weight: 1
tags: ["NodeJS", "NPM", "JSON"]
categories: ["Notes"]
date: 2020-07-25
draft: false
author: "Prajwal"
authorLink: "https://prajwalyashasvi.in"
timeToRead: "5"
---

Using wildcards and Arthmetic operators in package.json file in package dependencies list <!--more-->

#### Wildcards

```JSON
// sample package.json

"dependencies": {
  "gatsby": "^2.23.3"
},
"engines": {
  "node": ">=10.15.0"
}
```

- `~`: if you write ~2.23.3, you want to only update releases like 2.23.xxxxx but not versions from 2.24.0

- `^`: if you write ^2.24.0, you want to update patch and minor releases: 2.24.2, 2.24.2 ..., 2.25.0 and so on but not from 3.0.0.

- `*`: if you write \*2.23.3, that means you accept all updates including 3.0.0, 4.0.0 and so on.

- `latest`: want to use the latest version available.

#### Arthmetic Operators

- `>=` or `>`: accept any version equal to or higher than the one you specify

- `<=` or `<`: accept any version equal or less than the one specified.
