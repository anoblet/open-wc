Updated provides a weakmap of updated properties.

```
updated(changedProperties) {
  console.log(changedProperties);
```

To check if a property has changed, use the get method:

```
updated(changedProperties) {
  if(changedProperties.get("prop")) ...
}
```

Keep in mind changedProperties provides the previous values of properties. To get the updated value, use ```this```.

```
updated(changedProperties) {
  const previousValue = changedProperties.get("prop");
  const newValue = this.prop
}
```
