### javascript
[javascript MDN](https://developer.mozilla.org/ko/docs/Web/JavaScript)

>##### Nullish coalescing operator
```
function print(foo) {
  const message = text || 'bar';
  console.log(message);
}

print('Foo');
// expected output: "Foo"
print(null);
// expected output: "bar"
print(undefined);
// expected output: "bar"
print(0);
// expected output: "bar"
print('');
// expected output: "bar"

const foo = null ?? 'default string';
console.log(foo);
// expected output: "default string"

const baz = 0 ?? 42;
console.log(baz);
// expected output: 0
```
[Nullish coalescing operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Nullish_coalescing_operator)
