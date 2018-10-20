Vue Typescript Method Styles Demo
=================================

`vue-property-decorator`对typescript的方法声明支持不全面。

下面两种写法，只有第1种正常支持。

```
showMessage1() {
  alert(this.message)
}
```

```
showMessage2 = () => {
  alert(this.message)
}
```

第二种不能正确的拿到修改后的`message`的值。
