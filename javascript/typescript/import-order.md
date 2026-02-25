# Import order

NOTES:

  - `type` last (`import type`)
  - Import variations:
    - Side effect (`import SOURCE`)
    - Default (`import ITEM from SOURCE`)
    - Individual (`import { ITEM } from SOURCE`)
    - Namespace (`import * as ITEM from SOURCE`)
  - Directory nesting:
    - Local (`./file.ts`)
    - Nested...
      * `./dir/file.ts`
      * `./dir/dir/file.ts`
    - Parenting...
      * `../file.ts`
      * `../../file.ts`
    
