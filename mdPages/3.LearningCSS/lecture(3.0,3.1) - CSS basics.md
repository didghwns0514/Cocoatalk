# CSS basic

## 1) CSS basic

- This gives style to HTML
- This can be placed with in the same file as HTML  
  or can be placed in a separate CSS file.

  ***

  > NOTE : To do this, use link tag to link style sheet.
  >
  > - href : To show location to the file.
  > - rel : describe the relation of the href file with the HTML.
  >   Here you show that it is "stylesheet" so css can be interpereted.
  > - With one .css file, you can apply this to many ther HTML for reusability.

### 1. External CSS

```HTML

<head>
  ...

  <link href="style_extern.css" rel="stylesheet" />

  ...
</head>

```

### 2. Internal CSS

```HTML
<head>
  ...
  <style>
    CSS code here...
  </style>

</head>

```

### 3. Inline CSS

```HTML
<p style="CSS style"></p>

```

## 2) How CSS works

1. Selector : Points, other words, selects tag.
2. Changes the design of the CSS.

## 3) CSS syntax

```CSS
h1 {
  color: blue;
  font-size:20px;
  ....
}

```

1. No spaces in the name of the attribute.
2. Each line should end with semicolon.
3. "Attribute" : "Attribute value"
