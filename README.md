# qa-addons

A public repository the IncubaCloud QA walks deploy from. It holds one
minimal Odoo 19 module, so a walk can check that an instance built from a
GitHub repository carries that repository's code, that a push rebuilds it
and that a pull request gets its own preview staging.

Nothing here is meant for use. Branches:

- `19.0`: what a production instance deploys.
- `qa-preview`: one commit ahead of `19.0`, the head of the pull request
  the walks open (by a signed webhook delivery; no real pull request is
  needed).
