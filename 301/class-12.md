### Class 12 Reading Notes

## EJS Partials

EJS allows for templating partials. Partials are chunks of HTML that can be used across multiple views.

To add a partial into a view, start by adding the HTML snippet to a .ejs file. Then, in the view you want to include it in, reference it with the EJS tags: `<%- include(partials/navbar) %>`. This line would add the partial stored in 'partials/navbar.ejs' into the view.

And that's basically it, you're good to go!

[Return to table of contents](../README.md)
