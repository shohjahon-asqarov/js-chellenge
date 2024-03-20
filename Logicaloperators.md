<!-- start time 11:50 21.03.2024 -->

Case: || , && , ! , ?? ,

|| (or) (yoki)
Shartlarni o'qishni boshlaydi agar true value topsa birinchi truthy qiymatni qataradi agar topa olmasa
eng oxirgi falsy qiymatni oladi. Bu matematikada + ga o'xshaydi. Ya'ni 0+0+0+1 buning natijasi bir (true)

&& (and) (va)
Shartlarni o'qishni boshlaydi agar falsy value topsa birinchi topgan falsy qiymatni qataradi. Bu opetatorda barcha qiymatlar true bo'lishi kerak.Bu matematikada * ga o'shaydi. Ya'ni ko'paytmaga bitta 0 qo'shilda natija 0 ga teng bo'ladi ya'ni false. 1*1*1*0=0.

! not
Berilgan qiymatni teskari tomonga o'giradi.
Misol: !true = false , !false - true

!!
Bu operator qiymatni booleanga o'zgartiradi.
!!"non-empty string" // true === Boolean("non-empty string")
!!null // false === Boolean(null)

?? nulish
null va undefined ga tekshiradi agar qiymat null yoki undefined ga teng bo'lmasa keyingi qiymatni oladi
a ?? b
if(a !== null && a !== undefined){
    return b
} 

<!-- end time 12:15 21.03.2024 -->
