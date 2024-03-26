<!-- 11:30 25.03.2024 -->

Iterable - takrorlanuvchi qiymatlar ya'ni fo(of) orqali qiymatlarini olish mumkun bo'lgan objectlar.

Obyektlani ham iteratsiya qilish mumkun [Symbol.iterator] orqali

const obj = {
name: "Someone",
age: 17,
[Symbol.iterator]: function () {
let index = 0;
let values = Object.values(this);
return {
next() {
if (index < values.length) {
const values = values[index];
index++;
return { done: false, value: value };
}
else {
return { done: true, value: values[index] }
}
}
}
}
}

let person = {
name: 'John' ,
age: 18
}

for (let [key, value] of Object.entries(person)) {
console.log(key, value);
}

<!-- 11:40 25.03.2024 -->
