# UpDwn Auto-change Title Hack

http://updwn.co/

```javascript
var myTitle = 'Jen Page (all rooms named Jen Page)';
var id = '-KAKt5llsPClHGzbQAtG';
function changeIt() {
  if ($('.edit[data-id=' + id).data('title') !== myTitle) {
    optionsRef.child(id + '/title').set('myTitle');
  }
  window.setTimeout(changeIt, 1);
}
```

Source: Jen Page
