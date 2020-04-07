---
template: post
title: 'Veb dasturlash uchun qo''llanma. Birinchi qism: Frontend'
slug: guide-to-web-development
draft: false
date: 2020-03-28T19:58:06.524Z
description: Veb dasturlashni yangi boshlovchilari uchun qo'llanma
category: 'web '
tags:
  - web
---
Bir necha kun oldin men nima uchun eslatib o'tilgan DevTrails loyihasini boshlashga qaror qilganim va birinchi qo'llanma ustida ishlashni boshlaganim haqida qisqacha esse yozdim. Mening shaxsiy ma'lumotimning aksariyati veb-ishlab chiqishda, shuning uchun men buni boshlash uchun yaxshi joy deb o'yladim. 

Shuningdek, bu boshlang'ichda ham, korxona sektorida ham talab katta bo'lgan sohaning eng katta segmentlaridan biri. Ushbu qo'llanma eng asosiy narsalardan boshlanadi, shuning uchun men boshlanuvchilar uchun qiziqroq bo'lishi mumkinligini his qilaman, ammo ma'lum tajribasi borlar  ham yangi narsalarni topishlari mumkin.



![](/media/18084e42cb065d08444d21d2ca16fe5d.jpg)

Yangi boshlanuvchilar uchun veb-ishlab chiqishga kirishish juda oson, chunki kirish darajasi nisbatan past bo'lgan ko'plab tillar, ochiq manbali bepul vositalar va rivojlanishni soddalashtiradigan ko'plab freymvorklar mavjud. Boshqa tomondan, tanlash uchun juda ko'p narsa bor. Dasturlashni qiyin tomoni shundaki, siz dasturni ishlashi uchun juda ko'p tarkibiy qismlarni birlashtirishingiz kerak. UI doirasini qaysi birini tanlash kerak? Ma'lumotlaringizni qayerda saqlash kerak? [PHP](https://www.php.net/), [Python](https://www.python.org/), [Ruby ](https://www.ruby-lang.org/en/)yoki boshqa biror narsa? Qanday qilib arizangizni qabul qilish kerak? Umid qilamanki, ushbu qo'llanma sizga ba'zi narsalarni ochib beradi va veb dasturlash borasida o'z yo'lingizni aniqlab olishga va hatto o'z karyerangizni boshlashga yordam beradi.

Qo'llanmani biz bir necha qismlarga ajratamiz va bugun biz birinchi qismdan boshlaymiz - [**Frontend** ](https://en.wikipedia.org/wiki/Front-end_web_development)dasturidan va sizni ushbu sohadagi eng muhim tillar va vositalar bilan tanishtiramiz.

### Front End dasturlash tillari va vositalari

Biz ushbu sohada sizni yo'naltirish uchun kamida bilishingiz kerak bo'lgan narsalarni ko'rsatadigan quyidagi xaritadan boshlaymiz:

![frontend xaritasi](/media/frontend_.png)

Frontend dasturlash (UI ishlab chiqarishi deb ham nomlanadi) veb-foydalanuvchi interfeyslarini, foydalanuvchi ko'radigan va o'zaro ta'sir qiladigan qismlarini yaratishni anglatadi. Frontend-ni ishlab chiqish uchta tamoyilga qattiq bog'langan: belgilash uchun [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML), pardozlash uchun [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS) va mantiq va o'zaro ta'sir qilish uchun [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript). Garchi ushbu uchta texnologiyalar vaqt sinovidan o'tgan bo'lsa-da, asosiy vositalar va tizim doimiy ravishda o'zgarib turadi. Ushbu qism sizga oldingi ekotizimni o'rganishni boshlash uchun boshlang'ich nuqtani beradi.

Frontend-ni ishlab chiqish, shuningdek, veb-dizayn va foydalanuvchi tajribasi (UX - user experience) bilan chambarchas bog'liq va har bir kompaniyada ikkala chegara har xil bo'lishi mumkin. Umuman olganda, frontend dasturchilar texnik muammolarga e'tibor berishadi, veb-dizaynerlar esa estetika va foydalanuvchi tajribasi (UX) bilan shug'ullanishadi. **UI** va **UX** lar haqida batafsil ma'lumot olish [](https://hackernoon.com/what-is-ui-ux-design-1f01e9dbbf02)uchun [bu yerni  bosing](https://hackernoon.com/what-is-ui-ux-design-1f01e9dbbf02)

#### HTML

[Hyper Text Markup Language (HTML)](https://developer.mozilla.org/en-US/docs/Web/HTML) bu foydalanuvchiga namoyish etiladigan ma'lumotni tuzishga imkon beradigan belgilash tili. Uning HTML hujjati har biri HTML yorlig'i bilan ifodalangan elementlardan iborat bo'ladi, masalan sarlavha, matn paragrafi yoki matn kiritish maydoni. HTML hujjatlari, shuningdek, giperhavola yordamida boshqa hujjatlar bilan bog'lanishi mumkin. Har bir teg o'ziga xos kontent turiga ega, ma'lum bir ko'rinishga va biriktirilgan xulq-atvorga ega. Agar siz HTML haqida biroz bo'lsa ham ma'lumotga ega bo'sangiz , juda oddiy statik HTML sahifalarini yaratishingiz mumkin bo'ladi.

##### CSS

[Cascading Style Sheets (CSS)](https://developer.mozilla.org/en-US/docs/Web/CSS) bu HTML elementlarining vizual ko'rinishini tasvirlash uchun ishlatiladigan uslublar tili. U elementning joylashishi, o'lchamlari, matn uslubi yoki ranglari yoki veb-saytning deyarli har qanday boshqa vizual jihatlari kabi jihatlarni boshqarish uchun ishlatilishi mumkin. Uslublar sahifadagi elementlar to'plamining bitta elementiga qo'llanilishi mumkin bo'lgan qoidalar to'plami sifatida belgilanadi. CSS-ning so'nggi xususiyatlari sizga asosiy stylingdan tashqariga chiqishga va animatsiyalar kabi murakkab vizual jihatlarni boshqarishga imkon beradi.

#### Pre-prosessorlar

CSS - bu kuchli til, lekin kodni qayta ishlatish va izolyatsiya haqida gap ketganda, uning cheklovlari mavjud. Shu sababli katta CSS kod bazasini saqlash qiyin bo'lishi mumkin. Ushbu kamchiliklarni bartaraf etish uchun dasturchilar guruhlari tomonidan bir qator yechimlar yaratildi. Ushbu tillar va ularning kompilyatorlari odatda CSS *protsessorlari* deb nomlanadi.

* [Sass / SCSS](https://sass-lang.com/) sizning CSS kod bazangizni yanada barqaror qilish uchun CSS imkoniyatlarini kengaytiradi. O'rnatish kabi ba'zi funktsiyalar CSS-ni kamroq og'zaki qiladi va yozishni osonlashtiradi, boshqalari esa o'zgaruvchilar va aralashmalar kodni qayta ishlatishga imkon beradi. Shuningdek, kodni kichikroq fayllarga bo'lib ishlashga imkon beradigan boshqa SCSS fayllarni import qilishni qo'llab-quvvatlaydi. [Compass ](http://compass-style.org/)kabi ba'zi mashhur CSS ramkalar Sass-ga asoslangan.
* [PostCSS ](https://postcss.org/)- bu CSS fayllarini o'zgartirish uchun JavaScript plaginlaridan foydalanadigan vositadir. Siz kod tahlilini amalga oshiradigan, o'zgaruvchan (variables) larni qo'llab-quvvatlashni qo'shadigan, kodni optimallashtiradigan va hokazo plaginlarni qo'shishingiz mumkin. Maxsus formatlar bo'lgan SCSS yoki Less-dan farqli o'laroq, PostCSS uchun standart CSS xususiyatlarini aks ettiradigan ko'plab plaginlar mavjud.
* [Less ](http://lesscss.org/features/)- Sass-ga o'xshash xususiyatlar to'plamiga ega bo'lgan pre-prosessor. Ularning o'xshashligiga qaramay, asosiy loyihalarda bir qator farqlar mavjud. Ilgari mashhur bo'lishiga qaramay, hozirda ko'plab dasturchilar Sass yoki PostCSS foydasiga Less-dan uzoqlashmoqdalar.

#### JavaScript

[JavaScript (JS)](https://developer.mozilla.org/en-US/docs/Glossary/JavaScript) - Internet uchun foydalanuvchi interfeyslarini ishlab chiqishda eng ko'p ishlatiladigan dasturlash tili. Bu foydalanuvchi veb-saytlariga foydalanuvchi xodisalariga munosabat, veb-xizmatlardan ma'lumotlarni yuklash va sahifadagi elementlarni ko'rsatish yoki yashirish kabi shaxsiy harakatlaringizni qo'shishga imkon beradi. Shuningdek, u turli xil API-lar orqali brauzer bilan o'zaro ishlashga imkon beradi. Siz uni veb-saytingizga alohida interfaol elementlarni qo'shish yoki murakkab veb-ilovalarni yaratish uchun ishlatishingiz mumkin. 

JavaScript bilan bog'liq boshqa bir atama ECMAScript bo'lib, aslida JavaScript uchun til tavsifidir. Ko'pgina hollarda, ular sinonim sifatida ko'rib chiqilishi mumkin.



#### Freymvorklar

JavaScript - bu kuchli til, ammo agar siz murakkab dastur yaratmoqchi bo'lsangiz, uni freymsiz ishlatsangiz, murakkab kod kodi paydo bo'ladi. Oddiy qilib aytadigan bo'lsak, u erda HTML-manipulyatsiya, ma'lumotlarni yuklash, dasturlarning umumiy arxitekturasi va boshqalar kabi asosiy funktsiyalarga yordam beradigan bir qator freynvorklar mavjud. Hozirgi kunda eng mashhur uchta freynvorklar - [React](https://reactjs.org/), [Angular ](https://angular.io/)va [Vue.js](https://vuejs.org/).

* [React ](https://reactjs.org/)- bu Facebook tomonidan ishlab chiqilgan foydalanuvchi interfeyslarini qurish uchun kutubxona. React tugmachalar yoki yon menyu kabi tarkibiy qismlarni yaratishga asoslangan bo'lib, kirish parametrlari asosida HTMLni namoyish eta oladi. React tarkibiy qismlari JavaScript kodi va HTML-ni qulay ravishda birlashtirishga imkon beradigan [JSX ](https://reactjs.org/docs/introducing-jsx.html)deb nomlangan JavaScript-ga kengaytma yordamida yozilgan. Murakkab interfeys elementlarini va butun dasturlarni yaratish uchun tarkibiy qismlar birlashtirilishi mumkin. React bu aslida freymvork emas, u faqat ko'rish qismini  ta'minlaydi, ammo uning boy vositalari va kutubxonalarining ekotizimida murakkab dasturlarni yaratish uchun kerak bo'lgan hamma narsa mavjud. Reactni boshlash juda oson, ammo vaqt o'tishi bilan sizda yetishmayotgan bo'shliqlarni to'ldirish uchun yangi kutubxonalarni o'rganishingiz kutiladi.
* [Angular](https://angular.io/)- tarkibiy qismga yo'naltirilgan "batareyalar kiritilgan" Google tomonidan ishlab chiqilgan freymvork turi. Angular dasturlari odatda TypeScript-da yoziladi. U veb-dasturni yaratish uchun kerak bo'lgan barcha narsalarni, shu jumladan CLI-ni ishga tushirish, loyihani ishlab chiqish va qurish uchun vositalarni, shuningdek shakllarni, ma'lumotlarni yuklash, marshrutlashni va boshqalarni boshqarish uchun kutubxonalarni yaratishni talab qiladi. U yuqori mavhumlik va murakkablik darajasiga ega va TypeScript-ni boshlang'ich rivojlanish tili sifatida o'rganish zaruriyatini yaratadi.
* [Vue.js](https://vuejs.org/) - bu modulli va bosqichma-bosqich qabul qilinishi mumkin bo'lgan tizim. Siz uni ko'rinish qismi sifatida foydalanishni boshlashingiz va kerak bo'lganda qo'shimcha kutubxonalarni qo'shishingiz mumkin. Boshqa freymvorklardan farqli o'laroq, eng muhim kutubxonalar asosiy Vue.js jamoasi tomonidan saqlanadi.

#### TypeScript

[TypeScript ](https://www.typescriptlang.org/)- statik turni tekshirish va async / await, sinflar yoki strelka funktsiyalari kabi so'nggi ECMAScript xususiyatlarini qo'shish uchun JavaScript-ni kengaytiradi. Natijada TypeScript kompozitsiyasi vanilil JavaScriptga aylanadi. Joylarda statik turni tekshirish kompilyator siz biron bir funktsiyani yoki o'zgaruvchini uning imzosiga mos kelmaydigan tarzda ishlatmoqchi bo'lganingizda sizni xabardor qiladi. Bu, shuningdek, kod muharrirlariga yaxshiroq kod navigatsiyasi va qayta ishlash qobiliyatini taqdim etish imkoniyatini beradi. Yozuvlar ixtiyoriy, shuning uchun ularni asta-sekin mavjud JavaScript loyihangizda tanishtirishingiz mumkin. TypeScript-dan foydalanish katta kodli bazalarga ega loyihalarda ishlashni ancha osonlashtiradi.



#### Komponentli kutubxonalar

Komponent kutubxonalari - bu komponentlarni yig'ishda ishlatilishi mumkin bo'lgan to'plamdir. Ulardan ba'zilari tugmachalar va ochilishlar kabi eng keng tarqalgan tarkibiy qismlarni amalga oshiradi, boshqalari murakkab sezgir (responsive) rejalarini yaratish uchun yordamchi dasturlarni taqdim etadi. Ularning har biri o'ziga xos vizual uslubga ega bo'lsa ham, ularni odatda sizning loyihangizning dizayni va brendiga mos ravishda moslashtirish mumkin. Ularning ko'plari oddiy CSS va JavaScript ko'rinishida mavjud, ammo ular ko'pincha boshqa mashhur JavaScript ramkalari bilan ishlash uchun yuboriladi. Ba'zi mashhur kutubxonalar:

* [Bootstrap ](https://getbootstrap.com/)- veb-ilovalarni yaratishda kuchli ramka. Bu tarkibiy qismlarning katta to'plami, shuningdek, sxemalarni yaratish uchun mavzular va vosita to'plamlari. Siz UI ni  komponentlarga qo'shishingiz mumkin, masalan, ochiladigan ro'yhat, JavaScript haqida minimal ma'lumot. Bootstrap yordamida qurilgan veb-sayt mavzularining keng tanlovi mavjud.
* [Semantic UI](https://semantic-ui.com/) - bu barcha turdagi komponentlarga va mavzularga ega bo'lgan boshqa mashhur UI kutubxonasidir. Shu bilan birga, tarkibiy qismlarni interfaol qilish uchun sizdan JavaScript kodini yozishingiz kerak bo'ladi.
* [Material UI](https://material-ui.com/) - Google-ning material dizaynidagi eng mashhur qo'llanma. U tarkibiy qismlar to'plamini, shuningdek, Google-ga muvofiq sizning ilovangiz qanday ko'rinishi va o'zini qanday tutishi haqida ko'rsatmalar beradi. 

  [Ant-d](https://ant.design/)esign, [Bulma ](https://bulma.io/)va [Pure ](https://github.com/pure-css/pure/)kabi ba'zi boshqa hurmatli eslatmalar.

#### Frontend qurollari

Frontend ekotizimi o'zining foydali maqsadlarga mo'ljallangan har bir vositasi bilan tanilgan. Ushbu qo'llanmada juda ko'p narsalar mavjud bo'lganligi sababli, biz ushbu qo'llanmada hamma narsani qamrab ololmaymiz, shuning uchun biz boshlash uchun muhim bo'lgan bir nechta narsalarga to'xtalamiz.



##### NPM

[Npm ](https://www.npmjs.com/)aslida ikkita narsani anglatadi:

1. Sizning loyihangizda o'rnatishingiz va foydalanishingiz mumkin bo'lgan minglab ochiq manbali kutubxonalar va vositalarni o'z ichiga olgan dasturiy ta'minot registri.
2. O'rnatish, yangilash va registrdan olib tashlash imkoniyatini beradigan CLI vositasi.



Npm-dan foydalanish sizning loyihangiz tomonidan foydalaniladigan kutubxonalarni o'rnatishingiz va ularni JSON fayliga hujjatlashtirishingiz mumkin. Ushbu faylni kod bazasi bilan birga saqlash sizning loyihangizga bog'liqliklarni aniq e'lon qilishingiz va ularni turli muhitlarga tezda o'rnatishingizni anglatadi. Bundan tashqari siz undan o'zingizning kutubxonalaringizni nashr qilish va boshqa dasturchilar bilan baham ko'rish uchun foydalanishingiz mumkin.

Npm-ga o'xshash narsa - bu [Yarn](https://yarnpkg.com/), u ba'zi yaxshilanishlarni va kutubxonani rivojlantirish uchun yaxshiroq qo'llab-quvvatlashni taklif qiladi va npm to'plamlari registriga mos keladi.

##### Webpack

[Webpack ](https://webpack.js.org/)-  mashhur modul to'plami. Bu sizga turli xil aktivlarni, masalan JavaScript kodi, CSS uslublari, HTML shablonlari va hatto rasmlarni brauzer tomonidan yanada samarali yuklanishi mumkin bo'lgan to'plamlarga birlashtirish imkonini beradi. Webpack-dan foydalanganda kodingizni modullarga ajratasiz. Har bir modul boshqa modullarni import qilishi mumkin. Keyin veb-paket import grafigini tahlil qiladi va resurslarni birlashtiradi. To'plamdan tashqari, Webpack to'plam kodini o'zgartirish uchun yuklovchilar va plaginlardan foydalanadi, masalan. tuzish, kod tahlili yoki minifatsiya qilish. Veb-paketni yaratish juda qiyin bo'lishi mumkin, ammo bu zamonaviy o'rnatishlarning aksariyati uchun asosdir.



##### Chrome Dev Tools

[Chrome DevTools ](https://developers.google.com/web/tools/chrome-devtools/)- bu Chrome brauzerida mavjud bo'lgan ko'plab vositalar to'plami. U nosozliklarni tuzatish holatlarida, masalan, dastlabki kodni yoki HTML elementlarini ko'rib chiqish, tarmoq so'rovlarini kuzatish va ilovangizning turli qismlarining ish faoliyatini o'lchash uchun ishlatilishi mumkin. Bu kichik sahifadagi o'zgarishlarni tezda sinab ko'rish uchun foydali bo'lishi mumkin bo'lgan sahifalarni tahrirlash imkonini beradi. Ushbu vositani puxta bilsangiz, son-sanoqsiz nosozliklarni xalos qilasiz. Shunga o'xshash vositalar boshqa brauzerlarda ham mavjud.

\---

Bu sizning frontend dasturlash yo'lida boshlashingiz uchun etarli bo'lishi kerak. Xavotir olmang, bu aysbergning uchi. Agar siz bu narsani batafsilroq o'rganishni xohlayotganingizni his qilsangiz, unda sizni juda ko'p qiziqarli narsalar kutmoqda.

\---

Manba: <https://medium.com/devtrailsio/beginners-web-development-guide-part-1-frontend-ca59f1877ec5> dan tarjima qilindi