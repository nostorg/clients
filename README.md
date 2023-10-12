## Viewing

View the deployed webpage [here](https://nostorg.github.io/clients/) or via the link in the sidebar.

## Contributing

Edit the landing page [here](index.md).

Edit the clients table/CSV [here](_data/clients.csv).

Workspace settings are included for use with the [Edit csv](https://marketplace.visualstudio.com/items?itemName=janisdd.vscode-edit-csv) extension for VS Code.

For `git diff` on the CSV file, try [daff](https://github.com/paulfitz/daff):

```bash
pipx install daff
daff git csv
git diff
```

Serve locally for testing:

```bash
brew install asdf
asdf plugin add ruby
asdf install # install ruby from .tool-versions
asdf exec bundle install # install from gemfile
asdf exec jekyll serve
```
