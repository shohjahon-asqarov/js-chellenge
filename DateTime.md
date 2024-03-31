<!-- 5:20 31.03.2024 -->

new Date() - bu vaqtni olihs uchun ishlatiladi.

let now = new Date();
alert( now ); // hozirgi vaqtni olib beradi

new Date(milliseconds) - 1970-yil 1-yanvardan boshlab to hozirgach abo'lgan millisecondllarni qaytaradi

<!-- metodlari -->

getFullYear() - yil
getMonth() - oy
getDate() - kun
getHours() - soat
getMinutes() - minut
getSeconds() - second
getMilliseconds() - millisecond
getDay() - hafta kuni
larni olish mumkun

<!-- codlarni qancha vaqt olayotganini bilish mumkun -->

let start = new Date(); // start measuring time

```
// do the job
for (let i = 0; i < 100000; i++) {
let doSomething = i _ i _ i;
}

let end = new Date(); // end measuring time

alert( `The loop took ${end - start} ms` );
```

<!-- 5:40 31.03.2024 -->
