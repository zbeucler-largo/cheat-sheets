## Tips

#### Pass by `value` vs pass by `reference`
- **Pass by reference**
  - `Boolean`
  - `Array`
  - `Function`
  - `Object`

- **Pass by value**
  - `pretty much everything else`

```mermaid
graph LR;

A[var X = ] --> C[" { prop: 'val' } "]
B[var Z = ] --> C[" { prop: 'val' } "]
```

- **How to test if a variable is a reference**
  - ```javascript
        var the_same = var1===var2;
        Object.is(var1, var2);
    ```



#### Libraries
- [wtfnode](https://www.npmjs.com/package/wtfnode)
