# package typejson

`import "typejson"`

## Index

- [class TypeJSON]()
  - [func parse(target: any, types: Types = {}): any]()
- [Type TypeJSONClass]()
- [Type Types]()


## class TypeJSON

### func parse

`parse(target: any, types: Types ={}): any`

Use types parse object

**Example**

```ts
// Validate required
expect(function () {
  tjson.parse({}, {
    "name": {
      type: "string"
    }
  })
}).toThrow(
  new Error(`typejson: attr: "name" is requried and must be a string`)
)
```
