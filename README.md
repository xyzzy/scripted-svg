# Welcome to Javascript Animated SVG graphics

Example of embedded javascript in a `SVG` image. Coding `SVG` is like coding `HTML` canvas.

Note that the script is only executed if the `SVG` is viewed directly in a javascript enabled player (browser) or embedded in `HTML` with the `<embed>` element.

The inspiration to create this was to add sandboxed javascript to github/gitlab/gitea `README.md` files.
However, only after creation it turns out that it does not work with `<img>` elements and `README.md` does not allow `<embed>`.

Parked here for historics and inspirations.

# Demonstration

<p>The SVG is interactive. You can drag the black pads to change the curve.</p>

<p>You need to host the `SVG` image on gh-pages.</p>

<p>Referencing the repository version will not work as GitHub does not consider `SVG` an image.</p>

<p>Standard `README.md` links do not open in a new window.</p>

<p>Some suggested ways of using a `SVG` image (size is 500x500):</p>

<dl>
<dt>Inline image (with javascript disabled) wrapped in whatever you please</dt>
<dd>

```html
<img src="scripted-svg.svg" width="200" height="200" alt="SVC">
```

<img src="scripted-svg.svg" width="200" height="200" alt="SVC">
</dd>

<dt>Inline image (with javascript enabled) wrapped in whatever you please</dt>
<dd>

```html
<embed src="https://xyzzy.github.io/scripted-svg/scripted-svg.svg" type="image/svg+xml">
```

<embed src="https://xyzzy.github.io/scripted-svg/scripted-svg.svg" type="image/svg+xml">

<p>NOTE: Will only work in `HTML` as `README.md` removes `<embed>` tags, Otherwise: `SVG` is interactive, you can move the black pads to change the curve.</p>
<p>NOTE: Avoid loading from `raw.githubusercontent.com`, it sends the `HTTP` header `"Content-Security-Policy: default-src 'none'; style-src 'unsafe-inline'; sandbox"` which disables the javascript.</p>
</dd>

<dt>For `README.md` combine both, javascript disabled preview that opens new tab with enabled version</dt>
<dd>

```html
<a href="https://xyzzy.github.io/scripted-svg/scripted-svg.svg" target="_blank"><img src="scripted-svg.svg" width="200" height="200" alt="SVC"></a>
```

<a href="https://xyzzy.github.io/scripted-svg/scripted-svg.svg" target="_blank"><img src="scripted-svg.svg" width="200" height="200" alt="SVC"></a>

<p>NOTE: The `SVG` when opened will full-screen.</p>
</dd>

<dt>Wrap the `SVG` with HTML to apply styling</dt>
<dd>

```html
<a href="https://xyzzy.github.io/scripted-svg/scripted-svg.svg" target="_blank"><img src="scripted-svg.svg" width="200" height="200" alt="SVC"></a>
```

<a href="https://xyzzy.github.io/scripted-svg/scripted-svg.html" target="_blank"><img src="scripted-svg.svg" width="200" height="200" alt="SVC"></a>
</dd>
</dl>

# Requirements

*   none

# Installation

*   none

# Versioning

Using [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/RockingShip/scripted-svg/tags).

# License

Everything withing `<script>` and `</script>` is part of `ccbc` and is licensed under the GNU Affero General Public License v3 - see the [LICENSE.txt](LICENSE.txt) file for details.
Everything else (the important stuff) is MIT.

## Acknowledgments

* W3C for their amazing work on SMIL and the browsers implementing it.
* Originating project [https://github.com/RockingShip/ccbc](https://github.com/RockingShip/ccbc)
