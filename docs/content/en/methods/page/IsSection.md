---
title: IsSection
description: Reports whether the given page is a section page.
categories: []
keywords: []
params:
  functions_and_methods:
    returnType: bool
    signatures: [PAGE.IsSection]
---

The `IsSection` method on a `Page` object returns `true` if the [page kind](g) is `section`.

```text
content/
├── books/
│   ├── book-1/
│   │   └── index.md  <-- kind = page
│   ├── book-2.md     <-- kind = page
│   └── _index.md     <-- kind = section
└── _index.md         <-- kind = home
```

```go-html-template
{{ .IsSection }}
```
