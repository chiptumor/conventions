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

The header is mandatory, excluding the scope. A type, followed by a colon, and a description must be included. A scope is optional, surrounded by parenthesis, can be inserted between the type and colon.

### Casing

A header's casing should be all lowercase except for references such as a variable name.

The following examples would be unconventional:

```plain text
Feat: Add file
```

```plain text
FEAT: add file
```

```plain text
feat: Add File
```

The following example would be a conventional equivalent:

```plain text
feat: add file
```

However, because the following example references a variable and class name, the capitalization doesn't affect the conventionality:

```plain text
feat: add ROOM_PRICE to HotelBooking
```

### Types

A commit message should begin with a type. There are a number of types to use&mdash;most commonly `feat` and `fix`, among several others (see [header/types](./header/types))&mdash;and you can use [scopes](#scopes) to improve specifics if necessary.
