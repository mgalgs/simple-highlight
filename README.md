## simple-highlight.el
*Extremelly simple highlight functionallity.*

---

This package provides functionality for highlighting the thing at point.
Multiple calls to the highlight function will result in changing the
highlight color. There is also

### Requirements


This package was tested for GNU Emacs 24.4 and above. Older Emacsen should
work but I have not tested with them.

### Installation


You can install via `MELPA`, or manually by downloading `simple-highlight.el`
and adding the following to your init file:

```elisp
(add-to-list 'load-path "/path/to/simple-highlight")
```

### Usage


Just require `simple-highlight` somewhere in your init file:

```elisp
(require 'simple-highlight)
```

See the [Function Documentation](#function-documentation) for more details.

this be simple test


I suggest you to add keybindings to the following functions:

```elisp
(global-set-key (kbd "C-c p h") 'simple-highlight-at-point)
(global-set-key (kbd "C-c p u") 'simple-highlight-unhighlight-at-point)
(global-set-key (kbd "C-c p U") 'simple-highlight-unhighlight-all)
```

### Customization


You can change the faces you want to use for highlight by setting the
variable `simple-highlight-faces`. For example:

```elisp
(setq simple-highlight-faces '(hi-green hi-yellow hi-blue))
```

### Changelog


1.0 - First release. <br/>

### Function Documentation


#### `(simple-highlight-next-highlight-face)`

Gets the next highlight face from list.

#### `(simple-highlight-at-point)`

Highlight the sexp at point.
The color of the highlight is changed with each highlighting.

#### `(simple-highlight-unhighlight-at-point)`

Unhighlight the sexp at point.

#### `(simple-highlight-unhighlight-all)`

Unhighlight all the highlights in current buffer.

-----
<div style="padding-top:15px;color: #d0d0d0;">
Markdown README file generated by
<a href="https://github.com/mgalgs/make-readme-markdown">make-readme-markdown.el</a>
</div>
