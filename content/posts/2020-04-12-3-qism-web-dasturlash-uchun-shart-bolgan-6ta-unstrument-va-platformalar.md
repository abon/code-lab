---
template: post
title: '3-QISM: Web dasturlash uchun shart bo''lgan 6ta unstrument va platformalar'
slug: web-dev-tools
draft: false
date: 2020-04-12T18:34:27.211Z
description: Web dasturlashda boshlovchilar uchun shart bo'lgan instrumentlar
category: web
tags:
  - devtools
---


> Ushbu post web dasturlashni yangi boshlovchilar uchun mo’ljallangan postlarning uchinchi qismi.[ **"1-QISM: FRONTEND"**](https://www.abdulloh.codes/posts/frontend-dev-guide),**[ "2-QISM:BACKEND"](https://www.abdulloh.codes/posts/backend-dev-guide)**

![thirdstep](/media/andrew-welch-q0-tdhboz4u-unsplash.jpg "foto: unsplash")



Webdasturlashni o'rganish bo'yicha suhbatimizni davom ettirar ekanmiz, biz ba'zi bir dasturlash tillaridan uzoqlashamiz va aksincha web-dasturlar ishlaydigan va ishlab chiqiladigan muhitga e'tiborimizni qaratamiz.



> Bu post boshlovchilar uchun bo'lgani sabab, instrumentlar ro'yhatini ham shunga moslab, hozircha eng keraklilarini saralab oldik. Tajribangiz oshishi bilan, mukammalroq instrumentlarni ham berib boramiz, Xudo xohlasa.



#### 🛠 Dasturlash Instrumentlari

![webtools](/media/images.png "foto: websitesetup.org")

Dastlab dasturni tuzatishda va kodni tuzishda tezda muvaffaqiyatga erishishingiz uchun, o'zingizning rivojlanish vositalaringizga qulay ekanligingizga ishonch hosil qiling. Siz ishlab chiqadigan har bir platformada ushbu platformaga tegishli ko'plab vositalar bo'ladi, ammo deyarli barcha ishlab chiqaruvchilar foydalanadigan ba'zi bir vositalar mavjud. Keling, ular orqali o'taylik.

##### ✒Kod Muharrirlari

Kod muharriri har bir dastur ishlab chiqaruvchisining uyidir. Bu erda sehr paydo bo'ladi. Asosiy kod muharrirlari kodlarni ajratib ko'rsatish, qayta tiklash va disk raskadrovka qilish qobiliyatlari kabi eng zarur xususiyatlar to'plamini ta'minlaydi. Bundan tashqari, integratsiyalashgan rivojlanish muhiti (IDE) deb nomlanuvchi, keng integratsiyalashgan vositalar va imkoniyatlarga ega bo'lgan yanada rivojlangan muharrirlari mavjud. Bu erda yeng mashhur kod muharrirlari:

* 🖋 [Visual Studio Code ](https://code.visualstudio.com/)- bu Microsoft tomonidan yaratilgan bepul o'zaro faoliyat platforma kodlari muharriri. U JavaScript, TypeScript, CSS va HTML uchun o'rnatilgan qo'llab-quvvatlashga ega, kengaytma sifatida ko'plab boshqa tillarni qo'llab-quvvatlaydi. VS Code sintaksisni yoritishni, kodni to'ldirishni, kodni yaratish uchun kod parchalarini, qayta ishlash qobiliyatlarini va o'rnatilgan terminalni taklif etadi. Shuningdek, dasturda xatolarni bartaraf etishga yordam beradigan o'rnatilgan tuzatuvchiga ega. Ushbu xususiyat tijorat IDE-laridagi kabi keng bo'lmasligi mumkin, ammo boshlash uchun yetarli.
*  🖋JetBrains IDE - bu turli platformalar uchun JetBrains tomonidan ishlab chiqilgan IDElar oilasi. Orqa tomonni ishlab chiqish uchun [WebStorm](https://www.jetbrains.com/webstorm/), Java uchun[ Intellij IDEA](https://www.jetbrains.com/idea/), PHP uchun [PhpStorm ](https://www.jetbrains.com/phpstorm/)va boshqalar mavjud. Ularning har biri tegishli tillar, freymvorklar va boshqa vositalarni qo'llab-quvvatlashga qaratilgan. Buni yanada foydali funktsiyalar bilan to'ldiring, masalan, versiyani boshqarish tizimlari bilan integratsiya, mahalliy o'zgarish tarixi yoki ishlaydigan vazifalar, va siz yuqori samarali ish muhitiga ega bo'lasiz. Ushbu mahsulotlar uchun pul to'lanadi, ammo[ IntelliJ Community Edition](https://www.jetbrains.com/idea/download/#section=windows)-dan bepul foydalanish mumkin.
* 🖋 [Visual Studio IDE](https://visualstudio.microsoft.com/vs/) - bu Microsoft tomonidan ishlab chiqilgan tijorat IDE. U uchta taklif bilan keladi: bepul nashr, professional va korxona. Bu dasturlash tillarining keng doirasini va dasturlaringizni ishlab chiqish va tuzatish uchun turli xil vositalarni qo'llab-quvvatlaydi. Buning ustiga, boshqa Microsoft mahsulotlari va Azure yoki Azure DevOps kabi xizmatlari bilan foydali integratsiyani ta'minlaydi. C # va TypeScript - bu VS-ning birinchi darajali fuqarolari.

##### ⚙ Versiyalarni Boshqarish Tizimlari

![vcs](/media/version-control-system.png "foto:herewecode")

Versiyalarni boshqarish tizimlari (VCS) har bir ishlab chiqish jarayonida asosiy rol o'ynaydi. VCS sizga masofaviy omborda barcha kod o'zgarishlarining to'liq tarixini saqlashga imkon beradi. O'zgarishlar tarixini ko'rib chiqish, turli xil versiyalarni yoki eski versiyalar bilan solishtirish uchun siz omborni ko'rib chiqishingiz mumkin. Bir nechta ishlab chiquvchilar o'zlarining mahalliy kod bazalarini sinxron holda ushlab turadigan loyihada hamkorlik qilish uchun bitta omborga o'zgartirishlarni kiritishlari mumkin. 

Hozirgi kunda VCS kodlar bazasi uchun haqiqatning so'nggi manbai sifatida ishlatiladi va zamonaviy rivojlanish jarayonlarining asosi hisoblanadi. VCS tizimlarini buyruq satri interfeysi orqali ishlatish mumkin, ammo turli xil kod muharrirlari bilan integratsiyalashgan holda turli xil GUI mijozlari ham mavjud.


Ikkita mashhur versiyani boshqarish tizimi mavjud:

* 🗃 [Git ](https://git-scm.com/)- eng mashhur VCS. Bu taqsimlangan tizim bo'lib, foydalanuvchi omborxonadan nusxa ko'chirganda, u loyihaning to'liq tarixini oladi va u bilan oflayn rejimda ishlashi mumkin. Ba'zan foydalanuvchilar markaziy masofaviy omborxonadagi o'zgarishlarni nashr etishlari va boshqalar tomonidan kiritilgan o'zgarishlarni yuklab olishlari kerak. Git ombori joylashganligini tasdiqlovchi ko'plab xizmatlar mavjud. Ulardan eng mashhurlari [GitHub ](https://github.com/)va [BitBucket](https://bitbucket.org/).
* 🗃  [Subversion (SVN)](https://subversion.apache.org/) - bu boshqa versiyani boshqarish tizimi. Git-dan farqli o'laroq, SVN sizga faqat bitta filialni tekshirish imkoniyatini beradi. Boshqa filialga o'tish uchun siz uni uzoq ombordan yuklab olishingiz kerak bo'ladi. Garchi bu sohada hanuzgacha foydalanilayotgan bo'lsa-da, Git yanada ommalashgan va uning atrofida ko'plab vositalar va xizmatlar mavjud.



![done](/media/undraw_complete_task_u2c3.png "foto: undraw")



Ushbu postda biz asosan turli xil platformalarda ishlab chiquvchilar uchun foydali bo'lishi mumkin bo'lgan vositalar va platformalarga e'tibor qaratdik. Biroq, ma'lum bir platforma bilan ishlashni boshlaganingizda, siz o'zingizning kontekstingizda foydali bo'lgan ko'plab yangi vositalarni topasiz.

\    \*                   \*                     *

Keyingi safar, turli xil bulutlarni tarqatish (cloud deployment) imkoniyatlarini ko'rib chiqamiz, shunda siz o'zingizning ilovalaringizni joylashtirish uchun mos variantni tanlashingiz mumkin.





*manba:  medium.com/devtrailsio/beginners-web-development-guide-part-3-platforms-and-tools-46467c4cd033 dan tarjima qilindi.*