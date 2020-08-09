# EJS Language for Atom

The current package, language-ejs, is non-functional and needed to be improved into a working standard. This is EJS-2, the working EJS syntax highlighting grammar for the Atom editor.

## Overriding the HTML Syntax for EJS file types

Usually, when you have a defined `<html>` tag in your document, then even if the file type is .ejs HTML will still be used as the default syntax highlighting. You can override this by editing your Atom's core config.

Go to File > Config and fine the `core` section and add (or edit) this `customFileTypes` definition into it so your core now looks like this (plus whatever was originally there)

```cson
  core:
    customFileTypes:
      "source.ejs-2": [
        "ejs"
      ]
```

Now all EJS file types will use the proper syntax highlighting defined by this Atom package for EJS.

## Screenshot

![EJS Syntax Highlights for Atom](https://i.imgur.com/WywKj8h.png)
