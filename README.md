# test-form-data

> :ledger: Testing `FormData` object.

## How it works?

```html
<form>
    <input name="post-title" value="Foobar"/>
    <input type="submit">
</form>
```

```javascript
let $form = document.querySelector('form');
let data = new FormData($form);
data.forEach((value, key) => {
    console.log(value, key); // => "post-title", "Foobar"
});
```

## Not working on my code, why?

Probably you forget about `name` attribute in each input.

## License

[The MIT License](http://piecioshka.mit-license.org) @ 2017
