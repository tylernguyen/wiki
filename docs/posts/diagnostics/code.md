---
icon: material/code-braces
date:
  created: 2025-01-01
  updated: 2025-04-11
---

# Code

Samples of [Pygments](https://pygments.org/) Syntax Highlighting in :simple-materialformkdocs:{ .materialformkdocs } Material for MkDocs.

Inherits [mkdocs-material/reference/code-blocks/ :octicons-arrow-up-right-16:](https://squidfunk.github.io/mkdocs-material/reference/code-blocks/)

<!-- more -->

## JavaScript :simple-javascript:{ .javascript }

//// collapse-code

``` js title="JS"
/**
* JSDoc example
* @param {Object} block - The block to be processed.
* @param {string} cls - The class name to be added to the block.
*/
function $initHighlight(block, cls) {
  try {
    if (cls.search(/\bno\-highlight\b/) != -1) {
      return process(block, true, 0x0F) + ` class="${cls}"`;
    }
  } catch (e) {
    /* handle exception */
  }
  for (var i = 0 / 2; i <= classes.length; i++) {
    if (checkCondition(classes[i]) === undefined)
      console.log('undefined');
  }

  return (
    <div>
      <web-component>{block}</web-component>
    </div>
  )
}
```

////

## CSS :simple-css3:{ .css3 }

//// collapse-code

``` css title="CSS"
@font-face {
  font-family: Chunkfive; src: url('Chunkfive.otf');
}

body, .usertext {
  color: #F0F0F0; background: #600;
  font-family: Chunkfive, sans;
  --heading-1: 30px/32px Helvetica, sans-serif;
}

@import url(print.css);
@media print {
  a[href^=http]::after {
    content: attr(href)
  }
}
```

////

## HTML :simple-html5:{ .html5 }

//// collapse-code

``` html title="HTML"
<!DOCTYPE html>
<title>Title</title>

<style>body {width: 500px;}</style>

<script type="application/javascript">
  function $init() {return true;}
</script>

<body>
  <p checked class="title" id='title'>Title</p>
  <!-- here goes the rest of the page -->
</body>
```

////

## Python :simple-python:{ .python }

//// collapse-code

``` python title="Python"
import asyncio
import time
from datetime import datetime


async def custom_sleep():
    print(f"SLEEP {datetime.now()}\n")
    await asyncio.sleep(1)


async def factorial(name, number):
    f = 1
    for i in range(2, number + 1):
        print(f"Task {name}: Compute factorial({i})")
        await custom_sleep()
        f *= i
    print(f"Task {name}: factorial({number}) is {f}\n")


start = time.time()
loop = asyncio.get_event_loop()

tasks = [
    asyncio.ensure_future(factorial("A", 3)),
    asyncio.ensure_future(factorial("B", 4)),
]
loop.run_until_complete(asyncio.wait(tasks))
loop.close()

end = time.time()
print(f"Total time: {end - start}")
```

////

## YAML :simple-yaml:{ .yaml }

//// collapse-code

```yaml title="YAML"
variables:
- key: stringVariable
  type: xlrelease.StringVariable
  value: Hello world
- key: passwordVariable
  type: xlrelease.PasswordStringVariable
- key: booleanVariable
  type: xlrelease.BooleanVariable
  value: true
- key: numberVariable
  type: xlrelease.IntegerVariable
  value: 42
- key: listVariable
  type: xlrelease.ListStringVariable
  value:
  - One
  - Two
  - Three
- key: mapVariable
  type: xlrelease.MapStringStringVariable
  value:
    1: I
    2: II
    3: III
- key: setVariable
  type: xlrelease.SetStringVariable
  value:
  - Apples
  - Pears
  - Oranges
- key: listBoxVariable
  type: xlrelease.StringVariable
  valueProvider:
    type: xlrelease.ListOfStringValueProviderConfiguration
    values:
    - One
    - Two
    - Three
```

////

## JSON :simple-json:{ .foreground }

//// collapse-code

```json title="JSON"
{
    "id": "uuid",
    "id2": "id",
    "id3": "id",
    "title": "title",
    "text": "paragraph",
    "todo": "text",
    "name": "first-name",
    "city": "city",
    "country": "country",
    "last-name": "last-name",
    "age": "age",
    "phone": "phone",
    "grade": "decimal",
    "price": "price",
    "card": "credit-card",
    "aniversary": "date",
    "color": "choice red blue yellow",
    "friends": [
        {"repeat": 5},
        {
            "id": "index",
            "name": "first-name",
            "last-name": "last-name",
            "company": "company",
            "email": "email"
        }
    ],
    "check-ins":{
        "id": "id",
        "name": "full-name",
        "opened": "date",
        "users": [
            {"repeat": 5},
            {
                "id": "uuid",
                "index": "index",
                "married": "boolean"
            }
        ]
    }
}
```

////
