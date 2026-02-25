# Property Order

NOTES:

  - Order:
    - `abstract` first
    - `override` last
    - Index signature (`[key: any]: any`) last
    - Optional last (`property?: any`)
    - Types:
      - Property: `property: any`
      - Call signature: `(): any`
      - Constructor: `constructor ()`
      - Constructor signature: `new (): any`
      - Get accessor: `get property(): any`
      - Set accessor: `set property(): any`
      - Method: `property(): any`
    - `static` first
    - `readonly` first
    - Visibility:
      - `public`
      - `protected`
      - `private`
    - Alphabetical
