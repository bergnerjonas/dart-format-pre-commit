# Dart Format `pre-commit`

[`pre-commit`](https://pre-commit.com) hook for Dart files.

Add the following in your `.pre-commit-config.yaml`:
```yaml
- repo: https://github.com/bergnerjonas/dart-format-pre-commit
  rev: "master"
  hooks:
    - id: dart-format
    - id: dart-fix
    - id: flutter-analyze
```

You can also only include/exclude some files (defaults to only `.dart`, is a pattern):

```yaml
- repo: https://github.com/bergnerjonas/dart-format-pre-commit
  rev: "master"
  hooks:
    - id: dart-format
      files: lib/* # Only format source files
      exclude: lib/src/utils.dart # Exclude utils
```

