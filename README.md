# evil-indent-plus

<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-generate-toc again -->
**Table of Contents**

- [evil-indent-plus](#evil-indent-plus)
    - [Introduction](#introduction)
    - [Usage](#usage)
    - [Differences from evil-indent-textobject](#differences-from-evil-indent-textobject)

<!-- markdown-toc end -->

## Introduction

This is a continuation of
[evil-indent-textobject](https://github.com/cofi/evil-indent-textobject). It
provides six new text objects to evil based on indentation:

* `ii`: A block of text with the same or higher indentation.
* `ai`: The same as `ii`, plus whitespace.
* `iI`: A block of text with the same or higher indentation, including the first
line above with less indentation.
* `aI`: The same as `iI`, plus whitespace.
* `iJ`: A block of text with the same or higher indentation, including the first
line above *and* below with less indentation.
* `aJ`: The same as `iJ`, plus whitespace.

## Usage

Simply install the package. You should not have to load it explicitly, whether
before or after evil loads. So long as the autoloads are handled, it will work.

## Differences from evil-indent-textobject

The `evil-indent-textobject` package provides text objects that select lines
with the *exact* same indentation as the current line. Lines that are either
indented *more*, or which are empty, will interrupt the selection, contrary to
expected behaviour. This package correctly handles these cases.
