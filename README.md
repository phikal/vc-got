# vc-got

This is an Emacs VC back-end for the [Game of
Tree](http://gameoftrees.org/) version control system.

------

To start using it make sure that `vc-got` is within your `load-path`
and `Got` is in the `vc-handled-backends` list.

With `use-package` something like this should be enough:

```emacs-lisp
(use-package vc-got
  :load-path "/path/to/vc-got/"
  :defer t)
```

## Drawbacks

While I've been using this backend on a daily basis for the last
months, there are some rough edges.  Fetching updates in particular is
one action that *at the moment* is better to do by hand.  Pushing,
committing, blaming etc on the other hand are fully functional.

Note that pushing requires at least got 0.56, other functionalities
should work with older versions.


## Contributing

The long-term plan is to get this into Emacs (or ELPA at least).  This
means that to avoid possible problems, a GNU copyright assignment is
required.  It's really easy to get one (just send an email), and
having one will allow you to make further contribution to Emacs itself
or to various other packages.
