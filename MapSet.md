<!-- 14:16 26.03.2024 -->

Bular **js** ning data structurlari hisoblanadi . Tagi obyekt va o’zini hususiyatlari bor.

**Map** - Obyekt bilan deyarli bir hil. Bitta farqi key sifatida hohlagan tipdagi qiymatni berish mumkun. Masalan 1 obyektni key sifatida 2-esa value sifatida berish mumkun.

**Set** - “Unique” qiymatlaridan iborat **collection**. Ya’ni har bir qiymat **Set**’ning ichida 1 marta takrorlanadi va **Set**’da key bo’lmaydi.

**WeakMap** - **Map** bilan deyarli bir hil . **Map**dan farqi key sifatida faqat obyekt oladi va key haqida ma’lumot beruvchi metodlardan foydalanib bo’lmaydi.

**WeakSet** - **Set** bilan deyarli bir hil. **Set**dan farqi qiymat sifatida faqat obyekt oladi.

Structuralari

// yaratish
const myMap = new Map();

// data qo'shish
myMap.set("info", { name: "Sam", age: 36 });

// datani olish
console.log(myMap.get("info"));

// shu nomdagi keyni tekshirish

- myMap.has("info");

// elementlar hajmini olish
console.log("The no.of elements in a Map are " + myMap.size);

// datani o'chirish

myMap.delete("info"); // true

// loop
const map2 = new Map();
map2.set("name", "Sam");
map2.set("age", "36");

// loop
map2.forEach(function (value, key) {
console.log(key + "- " + value);

<!-- metods -->
new Map()- xaritani yaratadi.
map.set(key, value)– qiymatni kalit orqali saqlaydi.
map.get(key)undefined– agar keyxaritada mavjud bo‘lmasa , kalit orqali qiymatni qaytaradi .
map.has(key)- trueagar keymavjud bo'lsa, qaytaradi, falseaks holda.
map.delete(key)– elementni (kalit/qiymat juftligi) kalit yordamida olib tashlaydi.
map.clear()- xaritadan hamma narsani olib tashlaydi.
map.size– joriy elementlar sonini qaytaradi.

<!-- 14:27 26.03.2024 -->
