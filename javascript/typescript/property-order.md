# Property Order

NOTES:

  - Order:
    - `abstract` last
    - `override` last
    - Visibility:
      - `public`
      - `protected`
      - `private`
    - `static` last
    - `readonly` first
    - Index signature (`[key: any]: any`) last
    - Optional last (`property?: any`)
    - Types:
      - Call signature: `(): any`
      - Constructor: `constructor ()`
      - Constructor signature: `new (): any`
      - Property: `property: any`
      - Get accessor: `get property(): any`
      - Set accessor: `set property(): any`
      - Method: `property(): any`
