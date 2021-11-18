# ESE Beamer theme

LaTeX Beamer theme for Erasmus School of Economics based on the Microsoft Powerpoint template.


## Using the theme

See also the file `example.tex` for a working example on how to use the theme.

- Include `\usetheme{ESE}` in the preamble.
- Use `\ESEtitlepage` to generate the title page.

**Theme options**:

- `framenumbers`: Display slide numbers in the bottom right corner.
- `navigation`: Display a navigation bar on the left hand side.
- `nologo`: Do not display the Erasmus logo in the bottom right corner.
- `notes`: Include notes (generated with `\note{}` in between slides) in the final document.
- `sectiontitles`: Display a slide with the section title at the start of each section.

An example for using these options is given below:
```
\usetheme[framenumbers, sectiontitles]{ESE}
```


### Commands for mathematical notation

For mathematical notation inside math environments, the following commands are
available:

- `\mat{}`: For formatting matrices, e.g., `\mat{X}`.
- `\vect{}`: For formatting vectors, e.g., `\vect{x}`.
- `\obs{}`: For formatting observations, e.g., `\obs{x}`.


### Other commands

For writing about software, the following commands are available:

- `\proglang{}` For highlighting programming languages, e.g., `\proglang{[R](https://www.r-project.org/)}`.  Note that this has no effect if a sans serif font is already used, such as the default Beamer font.
- `\pkg{}` For highlighting software packages, e.g., `\pkg{[robmed](https://github.com/aalfons/robmed)}`.
- `\code{}` For highlighting functions, e.g., `\pkg{robmed()}`.

Special characters currently need to be escaped within those commands, e.g., `\_` for underscores so that function `test_mediation()` should be typeset as `\code{test\_mediation()}`.


### Official Erasmus colors

The ESE Beamer theme defines the following [official Erasmus colors](https://www.eur.nl/en/about-eur/house-style/brand-elements/colours):

- `EURbrightgreen` (for digital purposes): RGB 12/128/102
- `EURgreen`: RGB 0/35/40
- `EURwarmgrey`/`EURwarmgray`: RGB 227/218/216 (not really useful as this is a very light gray)
- `ESEyellow`: RGB 255/215/0

Command `\alert()}` uses `EURbrightgreen` for highlighting.  The remaining colors can be used with `\textcolor{}{}` to highlight text, e.g.:
```
\textcolor{EURgreen}{This is a very dark green (RAL 6012 black green).}
```


## Report issues and request features

If you experience any bugs or issues or if you have any suggestions for additional features, please submit an issue via the *Issues* tab of this repository.  Please have a look at existing issues first to see if your problem or feature request has already been discussed.


## Contribute to the package

If you want to contribute to the theme, you can fork this repository and create a pull request after implementing the desired functionality.
