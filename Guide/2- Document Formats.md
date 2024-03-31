## Document formats

##### In this second "class" I will explain how to format your LaTeX document.

##### The first information processed by LaTeX is what kind of document it should read, these kinds of documents are called **classes**, and they come in many shapes and sizes. Let's list them and explain them one by one:

1. **Document Classes** `\documentclass[options]{class}`

   1. _article_: For articles in cientific magazines, short documents, software documentation, invitations, etc.
   1. _proc_: For proceedings, based in the _article_ class.
   1. _minimal_: Is the smallest you can go, it establishes a unique page and font size, used for debugging.
   1. _report_: For longer articles that may contain chapters, small books and thesis.
   1. _book_: For books, what else?
   1. _beamer_: For slideshow

1. **Options inside Document Classes**
   1. _Font size_: Optional, custom set to 10pt.
   1. _Paper size_: A few possible options are: `a4paper`, `letterpaper`.  
      There are many options, for now, this two will suffice, the other ones will be introduced when necessary.

### How do we go about using all this?

In LaTeX every command has the prefix `\` attached to it, so if we want to write an article in A4 paper size with 10 pt font size what we do is **_AT THE TOP OF THE DOCUMENT_** write `\documentclass[a4paper]{article}`.

LaTeX will start reading the preamble of your document (the part before what you actually want to write in the doc) from top to bottom, for this, **the first line must always be the document class command**.

### Environments

Now that we have the document type it's time to add something to it. Just below your document class command we will use an **environment** called _document_.

All environments use the syntax:

```latex
\begin{environment name}
    % what we want to write inside the enviroment
\end{environment name}
```

And yes, you guessed right, `%` in latex is used for comments in the code. If we wanna use the symbol '%' what you do for LaTeX to render it is written it as `\%`.

#### The document environment

As said before, we will be using the _document_ environment to write all the text and things we want to appear in the doc. Let's do it! Try adding some dummy text to your document. In the end it should look something like this:

```latex
\documentclass[a4paper]{article}

% This is the preamble, we will know what to do here
%later in the guide.

\begin{document}
    Lorem ipsum dolor sit amet consectetur adipiscing elit dignissim dictumst eros.
\end{document}
```

And it looks like this:

<div align="center">
<img alt="example" src="../Assets/2-Document-Formats/Lorem.JPG">
</div>

In the [next section](https://github.com/Uklizdev/LaTeX-Guide/blob/master/Guide/3-%20Styling.md) we will learn how to style the page with a title, changing font sizes and a few types of spaces.
