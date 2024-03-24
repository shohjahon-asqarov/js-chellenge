<!-- start time 18:40 24.03.2024 -->

String - bu jsdagi mavjud data type

length - string uzunligi

eslatma
'text'[0] // 't'
'text'[0] = 'b' // error

<!-- upper lower case -->
alert( 'Interface'.toUpperCase() ); // INTERFACE
alert( 'Interface'.toLowerCase() ); // interface

<!-- methods -->
let str = 'Widget with id';

<!-- indexof - berilgan qiymat nechani o'rinda turgani qaytaradi -->
alert( str.indexOf('Widget') ); // 0,  'Widget' qiymati mavjud
alert( str.indexOf('widget') ); // -1, bu qiymat topilmadi

alert( str.indexOf("id") ); // 1, "id" qiymati topildi (..idget with id)

<!-- indexOf - 2 argument -->
let str = 'Widget with id';

alert( str.indexOf('id', 2) ) //  2-chi 'id' qiymati  12-indexda kelyapdi

<!-- included - berlgan qiymat string ichida bormi yo'qmi tekshiradi -->
alert( "Widget with id".includes("Widget") ); // true

alert( "Hello".includes("Bye") ); // false


<!-- start and end with -->
alert( "Widget".startsWith("Wid") ); // true, "Widget" starts with "Wid"
alert( "Widget".endsWith("get") ); // true, "Widget" ends with "get"


<!-- slice -->
let str = "stringify";
alert( str.slice(0, 5) ); // 'strin', the substring from 0 to 5 (not including 5)
alert( str.slice(0, 1) ); // 's', from 0 to 1, but not including 1, so only character at 0

<!-- end time 19:00 19.03.2024 -->
