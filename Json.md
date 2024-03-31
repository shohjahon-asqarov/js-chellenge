<!-- 5:46 31.03.2024 -->

# JSON methods, toJSON

```
let user = {
  name: "John",
  age: 30,

  toString() {
    return `{name: "${this.name}", age: ${this.age}}`;
  }
};

alert(user); // {name: "John", age: 30}
```

> [!NOTE]
> JSON (JavaScript Object Notation) qiymatlar va ob'ektlarni ifodalash uchun umumiy format.

- JSON.stringifyob'ektlarni JSONga aylantirish uchun.
- JSON.parseJSON-ni yana ob'ektga aylantirish uchun.

```
let student = {
  name: 'John',
  age: 30,
  isAdmin: false,
  courses: ['html', 'css', 'js'],
  spouse: null
};

let json = JSON.stringify(student);

alert(typeof json); // we've got a string!

alert(json);
/* JSON-encoded object:
{
  "name": "John",
  "age": 30,
  "isAdmin": false,
  "courses": ["html", "css", "js"],
  "spouse": null
}
*/
```

> [!NOTE]
> Objectni jsonga compile qilayoganda

-Funksiya xususiyatlari (usullari).
-Ramziy kalitlar va qiymatlar.
-Saqlaydigan xususiyatlar undefined.
bo'lgan vaziyatlarda bularni ignore qiladi

```
let user = {
  sayHi() { // ignored
    alert("Hello");
  },
  [Symbol("id")]: 123, // ignored
  something: undefined // ignored
};

alert( JSON.stringify(user) ); // {} (empty object)
```

<!-- 5:58 31.03.2024 -->
