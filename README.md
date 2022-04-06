# Breakable and Skippable For-Each Loops

Implementation example of a breakable and skippable For-Each loop. This kind of implementation imitates the functionality of the Continue, Skip, Next and Break statements.

Written in a theoretical programming language of my taste:

```ChiKleR's own programming language
## Returning false from the callback  skips that iteration.
## Returning  true from the callback breaks  the loop.
for_each := (

  collection : []Any | Object,
  cb : ( item : Any ) -> Bool

) -> Void {

  for item in collection
  {
    if cb(item) break;
  }
}
```

Note that this implementation is a mere generic example and may vary depending on the intention and the language.

Following this layout, you can build your own breakable and skippable For-Each loops, if the libraries you are using don't provide them.
