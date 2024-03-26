<!-- 14:33 26.03.2024 -->

Destructuring - bior element ichidan qiymatlani olish yo'llari

let arr = ["John", "Smith"]

let [firstName, surname] = arr;

alert(firstName); // John
alert(surname); // Smith

shunga o'xshaydi
let firstName = arr[0];
let surname = arr[1];

// ,, bunga e'tiborli bolish kerak
let [firstName, , title] = ["Julius", "Caesar", "Consul", "of the Roman Republic"];

alert( title ); // Consul

bu usullar faqta array uchun emas boshqa typelarda ham ishlaydi
let [a, b, c] = "abc"; // ["a", "b", "c"]
let [one, two, three] = new Set([1, 2, 3]);

// lopp jarayonida yordam beradi
for (let [key, value] of Object.entries(user)) {
alert(`${key}:${value}`); // name:John, then age:30
}

<!-- ... rest operator bilan ishlashi -->

let [name1, name2, ...rest] = ["Julius", "Caesar", "Consul", "of the Roman Republic"];

// rest is an array of items, starting from the 3rd one
alert(rest[0]); // Consul
alert(rest[1]); // of the Roman Republic
alert(rest.length); // 2

<!-- yana boshqa usullari -->

let options = {
title: "Menu",
width: 100,
height: 200
};

// { sourceProperty: targetVariable }
let {width: w, height: h, title} = options;

// width -> w
// height -> h
// title -> title

alert(title); // Menu
alert(w); // 100
alert(h); // 200

<!-- 14:42 26.03.2024 -->
