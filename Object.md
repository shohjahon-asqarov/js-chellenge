<!-- start time 5:12 23.03.2024 -->

Object bu nonprimative data type hisoblanadi. Object key va valuelardan tashkil topadi. Object ichida barcha primative data typelar kelishi mumkun.
Object yaratish yo'llari:
1 - new Object() // constructor syntax
2 - {} // literal syntax

Objectlarni primtive data typelardan farqi objectlar callstackda reference saqlaydi.
2 ta objectni solishtirganda bular hech qachon teng chiqmaydi , chunki bu ikki object xotirada boshqa boshqa adressda turgan bo'ladi.

<!-- check key -->

Object ichida berilgan key bor yoki yo'qligini tekshirish

let user = { name: "John", age: 30 };

alert( "age" in user ); // true, user.age exists
alert( "blabla" in user ); // false, user.blabla doesn't exist

<!-- sikl -->

let codes = {
"49": "Germany",
"41": "Switzerland",
"44": "Great Britain",
// ..,
"1": "USA"
};

for (let code in codes) {
alert(code); // 1, 41, 44, 49
}

<!-- delete key -->

delete user.age;

<!-- copy -->

let user = { name: 'John' };

let admin = user;

admin.name = 'Pete'; // changed by the "admin" reference

alert(user.name); // 'Pete', changes are seen from the "user" reference

bu yerda 2 o'zgaruvchi ham bir adressga murojat qiladi

<!-- clone -->

// 1
let user = {
name: "John",
age: 30
};

let clone = {}; // the new empty object

// let's copy all user properties into it
for (let key in user) {
clone[key] = user[key];
}

// 2
Object.assign(clone, user)

// ... spread operator
borqali ham clone olish mumkun lekin nested keylarda xatolikka olib keladi yani chuqur copy qilaydi.
let user = {
name: "John",
sizes: {
height: 182,
width: 50
}
};



<!-- end time 5:25 23.03.2024 -->
