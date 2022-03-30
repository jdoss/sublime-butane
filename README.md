# Sublime Butane

This is the repository for the [Butane](https://coreos.github.io/butane/) syntax and snippets files for the
[Sublime Text](https://www.sublimetext.com/) editor.

## Installation

### Prereqs

#### Package Control

1. [Install](https://packagecontrol.io/installation) Package Control

#### LSP and LSP-yaml
1. Open the command palette and run `Package Control: Install Package`, then select [`LSP`](https://packagecontrol.io/packages/LSP)
2. Install [`LSP-yaml`](https://github.com/sublimelsp/LSP-yaml) from Package Control
3. Restart Sublime

### Install with Package Control

1. Install *Package Control* for Sublime Text by following these instructions:
   https://packagecontrol.io/installation
2. Install the Butane package:
   `Preferences -> Package Control -> Package Control: Install Package`
   Type in `Butane` and hit Enter/Return

### Install Manually

Clone or download and extract this repo into your Packages directory which can be found by:
 `Sublime Text -> Preferences -> Browse Package`
￼
**Linux**: ~/.config/sublime-text-3/Packages
**MacOS**: ~/Library/Application Support/Sublime Text 3/Packages
**Windows**: %APPDATA%\\Sublime Text 3

### Configure LSP-yaml

Edit open `LSP-yaml/LSP-yaml.sublime-settings` by going to `Prefrences -> Package Settings -> LSP -> Servers -> LSP-yaml`
and add this override to make LSP-yaml read butane files (`.bu`):

```json
// Settings in here override those in "LSP-yaml/LSP-yaml.sublime-settings"

{
  "selector": "source.yml | source.yaml | source.bu"
}
```

## License

The MIT License

Copyright (c) 2022 Joe Doss

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
