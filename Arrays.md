<!-- start time 10:40 25.03.2024 -->

Array bu qiyatlar to'plami

Arrayni elon qilish usullari

<!-- new Array()  1 -->
<!-- [] 2 -->

<!-- Arrayda qiymatlar index bo'ylab joylashadi -->

<!-- arraydan qiymatni olish -->

let fruits = ["Apple", "Orange", "Plum"];

alert( fruits[0] ); // Apple
alert( fruits[1] ); // Orange
alert( fruits[2] ); // Plum

<!-- qiymatni o'zgartirish mumkun lekin stringda mumkun emas -->

fruits[2] = 'Pear';

fruits.length // 3 - bur orqali array ichidagi elementlar sonini bilish mumkun

<!-- Arraydan oxirgi elementni olish -->

let fruits = ["Apple", "Orange", "Plum"];
fruits[fruits.length-1] // Plum

at orqali

let fruits = ["Apple", "Orange", "Plum"];

fruits.at(-1) ; // Plum

<!-- pop , push , shift , unshift -->

push - oxiriga element qo'shadi.
pop - elementni oxiridan oladi.
shift - arrayning birinchi elementini chiqaradi va uni qaytaradi:
unshift - elementni massivning boshiga qo'shadi

<!-- splice() -->

let arr = ["I", "study", "JavaScript"];

arr.splice(1, 1); // 1 indexdagi qiymatni o'chiradi

alert( arr ); // ["I", "JavaScript"]

Bundan tashqari qiymatni o'chirib o'rniga boshqa qiymat biriktirish ham mumkun
let arr = ["I", "study", "JavaScript", "right", "now"];

// berilgan indexndagi elementlarni o'chiradi va o'rniga berilgan qiymatlarni qo'shib qo'yadi
arr.splice(0, 3, "Let's", "dance");

alert( arr ) // now ["Let's", "dance", "right", "now"]

<!-- end time 11:00 25.03.2024 -->
