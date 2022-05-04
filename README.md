# Markjam


A simple intermediate representation for plain text docs targeting HTML.
You can use it directly if you don't mind that it is weird.

```
[str obj? (str|arr)?]
```

```
[b [i "bolded and italicized"]]
```

```
[a {href https://...}
   click this bold green link]
```

```
[body { style max-width:72ch }
  [h1 Markjam]
  [p "
    A simple intermediate representation ...
    You can use it directly...
  " ]
  [ pre "[b [i \"bolded and italicized\"]]" ]
]
```