# Import order

NOTES:

  - `type` last (`import type`)
  - Import variations:
    - Side effect (`import SOURCE`)
    - Default (`import ITEM from SOURCE`)
    - Individual (`import { ITEM } from SOURCE`):
      - `type` last (`ITEM, type ITEM`)
    - Namespace (`import * as ITEM from SOURCE`)
  - Directory nesting:
    - Local (`./file.ts`)
    - Nested...
      * `./dir/file.ts`
      * `./dir/dir/file.ts`
    - Parenting...
      * `../file.ts`
      * `../../file.ts`
  - Alphabetical

    Example:

    ```ts
    import "./a-file.ts";
    import "./z-file.ts";
    import "./a-dir/file.ts";
    import "./z-dir/file.ts";
    import "./dir/a-dir/file.ts";
    import "./dir/z-dir/file.ts";
    import "../a-file.ts";
    import "../z-file.ts";
    import "../dir/file.ts";
    import "../../file.ts";
    import "../../dir/file.ts";

    import ITEM from "./file.ts";
    import { ITEM, type ITEM } from "./file.ts";
    import * as ITEM from "./file.ts";

    import type ITEM from "./file.ts";
    import type { ITEM } from "./file.ts";
    ```    
