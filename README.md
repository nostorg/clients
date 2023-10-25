## Viewing

View the deployed webpage [here](https://nostorg.github.io/clients/) or via the link in the sidebar.

## Contributing

Where to make changes:

- [landing page](index.md)
- [feature columns](_data/features.yml)
- [client row order](_data/order.yml)
- [client info & features](_data/clients/)

Serve locally for testing:

```bash
brew install asdf
asdf plugin add ruby
asdf install # install ruby from .tool-versions
asdf exec bundle install # install from gemfile
asdf exec jekyll serve
```
