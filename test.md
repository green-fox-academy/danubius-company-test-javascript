# Danubius Test

## Short questions

- What is the difference between `<span>` `<div>` and `<article>`?

- What similarities and differences do you know between
localStorage and cookies?

- What kind of HTTP methods are you familiar with?
What is the purpose of each of them?

- What will be the value of `x` after execution?

```js
var a = b = x = 0;
x = ++a + b++;
```

- What will be the value of `x` after execution?

```js
var x = (a = 3);
```

- What is the output **and why**?

```js
var bar = function() { console.log("bar"); }
var foo = function() { console.log("foo"); }
console.log("baz");
setTimeout(foo, 1000);
setTimeout(bar, 500);
```

- What is the difference between the 2 variables?

```js
var v1 = document.getElementById('inputText');
var v2 = $('#inputText');
```

- What are the possible ways to reference the variable
that holds `John Smith`?

```js
var data = {
  'person.name': 'John Smith'
};
```

- What is the output **and why**?

```js
var callbacks = [];
for (var i = 0; i < 5; ++i) {
  callbacks.push(function() { console.log(i); });
}

callbacks[3]();
```
- What is the output **and why**?

```js
var a = 2, b = { c: 4 };
var x = a, y = b;
x = 5;
y.c = 6;
console.log(a + b.c);
```

- What is the difference between the 2 CSS selectors?

```css
.element .symbol {}
.element.large .symbol {}
```

- What will be the color of the text **and why**?

```html
<div class="form-square">
  <div class="seven-col">
    Hello World!
  </div>
</div>
```

```css
div.form-square > div {
  color: blue;
}
.seven-col {
  color: red;
}
```

## Database scheme designing

Your task is to design the database scheme of a webshop
The database is relation so you should think in tables!

We'd like to store products in a way that admins can register
new products on a different view. A product could have any number
of attributes that could have any type. The requirement is
that in case of a new product type or a new product attribute
the scheme should not have to be modified

Examples for products and attributes:

### Dell Vostro X500

- memory: 16gb
- number of processor cores: 4
- release date: 2015-12-31

### Braun A1800 hair dryer

- color: black, white
- power: 1800W
- cold air blowing support: yes
- warranty period in months: 12

## Task

The goal is to create a structure in a way that if we'd like
to store the screen resolution of a notebook we don't have
to change the scheme of the tables. If you find more than
one solution you should can write more of them. You can write
the scheme in any way that we will understand :)
