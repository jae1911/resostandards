---
title: Wiki Release Page
author: Jae AKA J4 <j@j4.lc>
author_resonite: J4
---

# Wiki Release Page

This document describe how a wiki release page should be formatted.  
A template is provided for ease of use.

## The Standard

The page shall be named `Beta <VERSION NUMBER>` which is either obtainable through the official changelogs or the dashboard version facet and display the date of release as an ISO 8601 string. You can see the release date as an ISO string within the version number itself.

> For instance, for the version `2024.4.3.1170`, the page would be named `Beta 2024.4.3.1170` and the release date `2024/04/03`.

As with most wikis, the version name should be highlighted in bold using `'''` at the start of the article.

If the build is compatible with the previous version, link to the previous compatible version using `[[Beta {ver - 1}]]`.

If any notes were sent with the release, add the string `The following notes were sent by` followed by a link to the team member having written the notes, usually being Frooxius.

Each line of notes shall start with `:` to add an indent to the text.

Changes shall be displayed as a list with each category being a normal text. For instance:

```wikitext
Category:
* Change
```

If a GitHub issue ID is provided, link to the relevant issue in the parenthesis after the change description.

The page shall be tagged with the `Versions` category using `[[Category:Versions]]`.

## Template

```wikitext
'''Beta {ver}''' is a Resonite version released on {date}.

<OPTIONAL: It is compatible with the previous build, [[Beta {ver - 1}]].>

The following notes were sent by [[User:Frooxius|Frooxius]]:

: Message

Thing:
* fixed ([<LINK TO GITHUB> #238473847])

[[Category:Versions]]
```
