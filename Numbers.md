<!-- start time 10:35 24.03.2024 -->

Jsda numberlarni 2 turi mavjud

- Oddiy raqamlar
  -BigInt raqamlar

  7.3e9 = 7.3 va 9ta nol = 7_300_000_000

Js runtimeda sonlar 2 darajasi 32 gacha boradi.

Sonlarni toFixed() orqali yaxlidlash mumkun.
Masalan: 0.3000000004..toFixed(2) = 0.2

Sonlarni sanoq sistemasiga o'tkazish uchun toString() methodi mavjud.
Masalan: 255..toString(2) bu endi 2 lik sanoq sistemasiga o'tadi

Sonlarda metodlarni ishlatish

.. sonlarga to'g'ridan to'g'ri metodlani ishlatib bolmaydi ishlatish uchun .. qo'yish kerak
(3456).method sonlarni () ga o'rash

Sonlarni yaxshlitlash

Math.floor - pastga yaxlitlaydi
Math.ceil - teaga yaxshlitlaydi
Math.round - yaqin songa yaxshlitlaydi

Agar jsda raqamlar chegaradan o'tib ketsa infinite qaytaradi.

Songa conversion qilish ususllari
Number()
+''
parseInt('100.5px') = 100 songa o'giradi va yaxlitlaydi - birinchi raqam topa olmagan joyda to'xtaydi
parseFloat('100.5px') = 100.5 songa o'giradi

Bularni 2 ta argument berib ham ishlatish mumkun
alert( parseInt('0xff', 16) ); // 255
alert( parseInt('ff', 16) ); // 255

alert( parseInt('2n9c', 36) ); // 123456

Math methodlari
Math.random() - 0-1 orasidagi tasodifiy sonnni qaytaradi
Math.max() - eng katta raqamni qaytaradi
Math.min() - eng kichik raqamni qaytaradi
Math.pow(3 , 9) - darajaga ko'taradi 3 ning 9-darajasi

- <!-- end time 11:00 24.03.2024 -->
