Transpiler - LiveScript , TypeScript kabi tillardan codlarni js ga compile qiluvchi xususiyat.

Polifill - eski browserlarda qollab quvvatlanmaydigan xususiyatlarni ishlatib beruvchi xususiyat

<!-- Masalan ES6 codlarni ES5 ga o'girilish -->

// code
height = height ?? 100;

// transpiler ishlashi
height = (height !== undefined && height !== null) ? height : 100;
