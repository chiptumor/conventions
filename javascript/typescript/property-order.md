# Property Order

NOTES:

  - Order:
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

    Example:

    ```ts
    class Example {
      public                    (): any;
      public                    constructor ();
      public                    property: any;
      public                    property?: any;
      public                    get property(): any;
      public                    get property?(): any;
      public                    property(): any;
      public                    property?(): any;
      public                    [key: any]: any;
      public                    [key: any]?: any;
      public                    [key: any](): any;
      public                    [key: any]?(): any;
      public           readonly property;
      public    static          property;
      public    static readonly property;
      protected                 property;
      protected        readonly property;
      protected static          property;
      protected static readonly property;
      private                   property;
      private          readonly property;
      private   static          property;
      private   static readonly property;
    }
    ```
