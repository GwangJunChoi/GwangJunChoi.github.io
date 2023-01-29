### javascript
[javascript MDN](https://developer.mozilla.org/ko/docs/Web/JavaScript)
1. async await ( https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Statements/async_function )
2. arrow function ( https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Functions/%EC%95%A0%EB%A1%9C%EC%9A%B0_%ED%8E%91%EC%85%98 )
3. Promise pattern ( https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Promise )
4. closure ( https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Closures )
5. import & export ( https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Statements/import )
6. Template Literals ( https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Template_literals )
7. 구조 분해 할당 <br>
    ex. [ a, b, ...foo] = array(1,2,3,4,5) <br>
        { a, b, ...c } = { a:1, b:2 , c:3, d: 4}<br>
        ( https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment )
8. prototype chain ( https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Inheritance_and_the_prototype_chain )
9. scope ( block & function )(var, let, const, arrow function ) <br>
        ( https://poiemaweb.com/js-scope )

>##### Nullish coalescing operator
```
function print(foo) {
  const message = foo || 'bar';
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
