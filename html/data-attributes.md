# data-* attributes

If you want to store some extra information
within the HTML tag that has no visual representation
you can use `data-*` attribute. What is most important
you can use as many data attributes as you wish/need.

__HTML syntax__

```markdown
<article
 id="bicycles"
 data-columns="4"
 data-user-id="234"
 data-user-name="Kate">
 ...
 </article>
``` 
__JavaScript access__

```markdown
var article = document.getElementById('bicycles');

article.dataset.columns // "4" as String
article.dataset.user.id // "234" as String
article.dataset.user.name // "Kate" as String
```
`article.dataset.columns = 5` will change the attribute to 5.

__CSS access__

```markdown
To show user name:
article::before {
    content: attr(data-user-name);
}

To change style:
article[data-columns='4'] {
    width: 400px;
}
```
---
_Last update: 24 Mar 2018_ 