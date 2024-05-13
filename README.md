# Python project template

## tools

- flake8
- black
- autoflake

## vscode extensions

- ms-python.python
- ms-python.flake8
- ms-python.black-formatter
- ms-python.isort
- mikoz.autoflake-extension
- njpwerner.autodocstring
- LittleFoxTeam.vscode-python-test-adapter

## vscode settings

```json
{
  "[python]": {
    "editor.defaultFormatter": "ms-python.black-formatter",
    "editor.formatOnSave": true,
    "editor.codeActionsOnSave": {
      "source.organizeImports": "always"
    }
  },
  "autoflake-extension.ignore-init-module-imports": true,
  "autoflake-extension.remove-all-unused-imports": true,
  "isort.args": ["--profile", "black", "--line-length", "100"],
  "black-formatter.args": ["--line-length", "100"],
  "flake8.args": [
    "--max-line-length", "100",
    "--per-file-ignores", "__init__.py:F401"
  ],
  "python.analysis.indexing": true,
  "python.analysis.autoImportCompletions": true,
}
```
