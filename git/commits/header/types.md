# Types

Types are used to define what a commit affects.

The allowed types are based on the [Angular convention] (including some of [its older version], corresponding with [Conventional Commits]).

[Angular convention]: <https://github.com/angular/angular/blob/61614f6caa99c39d66e4a7a97834739589932414/contributing-docs/commit-message-guidelines.md>
[its older version]: <https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines>
[Conventional Commits]: <https://conventionalcommits.org/>

| Type         | Description ("this commit will...")              | Example |
| ----------   | ------------------------------------------------ | ------- |
| [`build`]    | Affect the build system or external dependencies | build(npm): install package |
| [`ci`]       | Affect CI configuration files and scripts        | ci(ga): configure github pages action |
| [`docs`]     | Affect documentation only                        | docs: explain getItem parameters |
| [`feat`]     | Add a new feature to the codebase                | feat(parser):  |
| [`fix`]      | Patch a bug in the codebase                      | (example) |
| [`perf`]     | Improve performance                              | (example) |
| [`refactor`] | Neither fix a bug nor add a feature              | (example) |
| [`style`]    | Not affect the meaning of the code               | Whitespace, formatting, missing semicolons |
| [`test`]     | Add missing tests or correct existing tests      | (example) |

[`build`   ]: #build
[`ci`      ]: #continuous-integration
[`docs`    ]: #documentation
[`feat`    ]: #feature
[`fix`     ]: #fix
[`perf`    ]: #performance
[`refactor`]: #refactor
[`style`   ]: #style
[`test`    ]: #test

## Build

Commits with the type `build` affect the build system or external dependencies.

### Examples

This commit makes the build system generate log files.

```plain text
build: export logs on build
```

### Examples with scope

This commit installs the Discord.js NPM package for Node.js.

```plain text
build(npm): install discord.js package
```

## Continuous Integration

Commits with the type `ci` affect CI (continuous integration) configuration files and scripts.

### Examples with scope

This commit sets up the GitHub Action that deploys to GitHub Pages.

```plain text
ci(ga): set up gh pages action
```

## Documentation

Commits with the type `docs` affect only the documentation.

### Examples

This commit writes an explanation of the `getItem()` function in the docs.

```plain text
docs: explain getItem() paramaters
```

## Feature

Commits with the type `feat` add a new feature to the codebase.

### Examples with scope

This commit allows the parser to parse arrays.

```plain text
feat(parser): support parsing arrays
```

## Fix

Commits with the type `fix` patch a bug in the codebase.

## Performance

Commits with the type `perf` improve performance.

## Refactor

Commits with the type `refactor` neither fix a bug nor add a feature.

## Style

Commits with the type `style` don't affect the meaning of the code.

### Examples

This commit adds missing semicolons to a file.

```plain text
style: add missing semicolons to main.js
```

### Examples with scopes

This commit adjusts the indentation of a function.

```plain text
style(whitespace): adjust indentation of stripNumbers()
```

This commit compresses the formatting of a JSON file.

```plain text
style(format): optimize config.json formatting
```

## Test

Commmits with the type `test` add missing tests or correct existing ones.
