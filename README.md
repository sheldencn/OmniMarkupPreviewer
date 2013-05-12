OmniMarkupPreviewer
===================

Description
-----------

OmniMarkupPreviewer is a plugin for both [Sublime Text 2] and [Sublime Text 3]
that preview markups in web browsers. OmniMarkupPreviewer renders markups into
htmls and send it to web browser in the backgound, which enables a live preview.
Besides, OmniMarkupPreviewer provide support for exporting result to
html file as well.

[Sublime Text 2]: http://www.sublimetext.com/2
[Sublime Text 3]: http://www.sublimetext.com/3

OmniMarkupPreviewer has builtin support following markups:

* [Markdown](http://daringfireball.net/projects/markdown/)
* [reStructuredText](http://docutils.sourceforge.net/rst.html)
* [WikiCreole](http://wikicreole.org/)
* [Textile](http://www.textism.com/tools/textile/)
* [Pod](http://search.cpan.org/dist/perl/pod/perlpod.pod) (Requires Perl >= `5.10`
  and can be found in `PATH`, if the perl version < `5.10`, `Pod::Simple` should be
  installed from `CPAN`.)
* [RDoc](http://rdoc.sourceforge.net/) (Requires `ruby` in your `PATH`)
* [Org Mode](http://orgmode.org) (Requires `ruby`, and gem `org-ruby` should be installed)
* [MediaWiki](http://www.mediawiki.org/) (Requires `ruby`, as well as gem `wikicloth`)
* [AsciiDoc](http://www.methods.co.nz/asciidoc/) (Requires `ruby`, as well as gem `asciidoctor`)


### Donation

If you find my work useful, please consider buying me a cup of coffee, all
donations are much appreciated :)

[![Donate via PayPal](https://dl.dropbox.com/u/2451120/donate-with-paypal.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=TD4HF4X2R53NE)
[![使用支付宝捐赠](https://dl.dropbox.com/u/2451120/donate-with-alipay.png)](https://me.alipay.com/timonwong)

Installation
------------

### With the Package Control plugin
The easiest way to install OmniMarkupPreviewer is through [Package Control].

[Package Control]: http://wbond.net/sublime_packages/package_control

Once you have Package Control installed, restart Sublime Text 2.

1. Bring up the Command Palette (<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd>
   on Windows and Linux. <kbd>⌘</kbd>+<kbd>⇧</kbd>+<kbd>P</kbd> on OS X).
2. Type "Install" and select "Package Control: Install Package".
3. Select "OmniMarkupPreviewer" from list.

The advantage of using Package Control is that it will keep OmniMarkupPreviewer
up to date automatically.


### Manual Install
**Without Git:**
[Download](https://github.com/timonwong/OmniMarkupPreviewer) the latest source
code, and extract to the Packages directory.

**With Git:**
Type the following command in your Sublime Text 2 Packages directory:

`git clone git://github.com/timonwong/OmniMarkupPreviewer.git`

The "Packages" directory is located at:

* **Windows:**  `%APPDATA%\Sublime Text 2\Packages\`
* **Linux:**    `~/.config/sublime-text-2/Packages/`
* **OS X:**     `~/Library/Application Support/Sublime Text 2/Packages/`


Usage
-----

### Key Bindings

The default key bindings:

**Windows, Linux:**

* <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>O</kbd>: Preview Markup in Browser.
* <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>X</kbd>: Export Markup as HTML.
* <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>C</kbd>: Copy Markup as HTML.

**OSX:**

* <kbd>⌘</kbd>+<kbd>⌥</kbd>+<kbd>O</kbd>: Preview Markup in Browser.
* <kbd>⌘</kbd>+<kbd>⌥</kbd>+<kbd>X</kbd>: Export Markup as HTML.
* <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>C</kbd>: Copy Markup as HTML.

### Command Palette

Available OmniMarkupPreviewer commands in the command palette:

* `OmniMarkupPreviewer: Preview Current Markup in Browser`
* `OmniMarkupPreviewer: Export Current Markup as HTML`
* `OmniMarkupPreviewer: Empty Cache`


What's New
----------

**For a complete list of changes, see [CHANGELOG.md](./CHANGELOG.md)**

**v2.0.1 (TBD)**

* Strip YAML frontmatter for Markdown files automatically.
* Check syntax name as well as filename extension for MediaWiki files.

**v2.0 (03/31/2013)**

* Added support for [Org Mode](http://orgmode.org) (Requires ruby, and gem
  `org-ruby` should be installed).
* Added support for [MediaWiki](http://www.mediawiki.org/) (Requires ruby, as
  well as gem `wikicloth`).
* Added support for [AsciiDoc](http://www.methods.co.nz/asciidoc/) (Requires ruby,
  as well as gem `asciidoctor`).
* Reviving view (redirecting to the new location) automatically after reconnected.
* Prevent Package Control for Sublime Text 3 installing this package as
  `.sublime-package` (zip archive).
* Fixed broken `ignored_renderer` setting.
* Improved Sublime Text 3 compatibility.

**v1.20 (03/15/2013)**

* Add support Sublime Text 3 (Experimental).
* Add new context command `Copy Markup as HTML`.
* Remove unused command `Sweep Cache (Remove Unused)`.
* Auto scroll now works correctly for documents contain images and MathJax equations.

**v1.12 (03/13/2013)**

* Renderes are now loaded asynchronously on startup (faster Sublime Text 2 startup).
* Add litcoffee support.


License
-------

This plugin released under MIT License:

    Copyright (c) 2013 Timon Wong

    Permission is hereby granted, free of charge, to any person obtaining a copy of
    this software and associated documentation files (the "Software"), to deal in
    the Software without restriction, including without limitation the rights to
    use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
    of the Software, and to permit persons to whom the Software is furnished to do
    so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in all
    copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.

Donors
------

[DONORS.md](./DONORS.md)
