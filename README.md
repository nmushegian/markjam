
# Markjam


A simple intermediate representation for plain text docs targeting HTML.
You can use it directly if you don't mind that it is weird.
A markjam object is a JAMS object with either one or two fields.
It either has just a element name, and the node value ('innerHTML'), like this:

```
{b {i "bolded and italicized"}}
```

Or it also has an `@` key which are the attributes for this node:

{ @ {id question class green}
  input "What color is this"  }



{ @ {style max-width:72ch}
  body {
    {h1 Markjam}
    {p [
      A simple intermediate representation for plain text docs targeting HTML.
      You can use it directly if you don't mind that it is weird.
      ...
    ]}
    {pre
      "{b {i \"bolded and italicized\"}}"
    }
    ...
}}