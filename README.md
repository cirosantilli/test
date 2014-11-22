Tests to see how Git web interfaces like GitHub and GitLab work exactly and to detect bugs with them.

This repository is mirrored at:

- <https://github.com/cirosantilli/test>
- <https://gitlab.com/cirosantilli/test>
- <https://bitbucket.org/cirosantilli/test>
- <https://sourceforge.net/projects/cirosantilli-test>
- <https://code.google.com/p/cirosantilli-test>
- <https://www.assembla.com/code/cirosantilli-test/git/nodes>

Tests that are very large will not be included here to keep this repository small:

- <https://github.com/cirosantilli/test-deep>
- <https://github.com/cirosantilli/test-diff-many-files>
- <https://github.com/cirosantilli/test-pr-many-commits>

There are also some tests that could not be included here conveniently:

- <https://github.com/cirosantilli/test-empty-commit>
- <https://github.com/cirosantilli/test-empty-subdir>
- <https://github.com/cirosantilli/test-long-filename-256>
- <https://github.com/cirosantilli/test-long-filename-1024>

Other similar repos from other people:

- <https://github.com/joernchen/evil_stuff>

The most interesting files on this repository are:

-   [markdown.md](markdown.md)

-   [issue-markdown.md](issue-markdown.md): test the markdown on issues

-   whitespace filename edge cases:

    - [single whitespace filename](%20)
    - [double whitespace directory name](%20%20/) and [its README](%20%20/README.md)
    - [a b](a b)

Interesting branches and tags:

-   [`hasslash/a`](../hasslash/a): branch inside sub-directory

-   [`-r`](../-r): branch with forbidden name, and in particular one that may be used for shell injection. 

-   `<script>alert('xss')</script>` and `<b>a</b>`: XSS and defacement attempts

    Create manually with `cp master -- -r` and push with `git push --all`.

-   `tag-empty-blob`
