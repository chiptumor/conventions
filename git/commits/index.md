# Commits

Chip's commit conventions are based mostly on [Conventional Commits].

[Conventional Commits]: <https://conventionalcommits.org/>

The regular layout of a commit message should look like this.

```plain text
<type>[scope?]: <description>

[body?]

[...footers?]
```

## Header

The header is mandatory, excluding the scope. A type, followed by a colon, and a description must be included. A scope, surrounded by parenthesis, can be inserted between the type and colon.

### Types

A commit message should begin with a type. There are a number of types to use&mdash;most commonly `feat` and `fix`, among several others (see [header/types](./header/types))&mdash;and you can use [scopes](#scopes) to improve specifics if necessary.
