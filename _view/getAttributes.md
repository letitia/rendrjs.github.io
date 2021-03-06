---
header: getAttributes
example: View.getAttributes()
---

Get the HTML attributes to be added to the element.  This will set the `id`, `attributes`, and `class` information; then adds `data-` to the keys for all options not included in [nonAttributeOptions](#nonAttributeOptions).

This returns an object with all the attribute names and values.

```js
var view = new View({ 'view-option': 'test' });
view.name = 'viewName';
view.className = 'text-muted';
var attrs = view.getAttributes();

// attrs
{
  'class': 'text-muted',
  'data-view': 'viewName',
  'data-view-option': 'test'
}
```
