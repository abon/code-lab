---
template: post
title: 'Web dasturlash uchun qo''llanma. 2-Qism: Backend'
slug: backend-dev-guide
draft: true
date: 2020-04-08T11:44:36.604Z
description: >-
  Boshlovchilar uchun Backend dasturchilikni boshlash uchun barcha kerakli
  ko'satma va instrumentlar.
category: web
tags:
  - web
---
> Ushbu post web dasturlashni yangi boshlovchilar uchun mo'ljallangan postlarning ikkinchi qismi. Birinchi qism bilan [bu yerda tanishing](https://www.abdulloh.codes/posts/frontend-dev-guide).

![runner](/media/jonathan-chng-mnsnlmhofpm-unsplash.jpg "foto: unsplash")

Bugun biz web dasturlar ishlab chiqish bo'yicha tanishuvimizni davom ettiramiz. Oldingi postda biz frontendni rivojlantirishni o'rganishdan boshladik va bugun biz orqa fonni, backend qismni rivojlantirish haqida gaplashmoqchimiz.

**Backend Development** (ba'zan *server tomoni* deb ataladi) serverda sodir bo'ladigan va odatda foydalanuvchilarga ko'rinmaydigan jarayonlarni ishlab chiqishni anglatadi. Veb-interfeys HTML-ni taqdim etish (renderlash) , ma'lumotlar bazasida foydalanuvchi ma'lumotlarini saqlash, foydalanuvchini tasdiqlash, elektron pochta xabarini yuborish yoki to'lovni amalga oshirishni so'rab, serverga so'rov yuboradi. Web ilovaning ushbu qismi foydalanuvchi uchun shaffof bo'lsa ham, hech qanday ahamiyatga ega emas. Bu sizning dasturingizning yuragi va miyasi.

![scheme](/media/1_1dss5h0uvhru5l1tl9irma.png "foto: medium")

#### Tillar

Frontend bilan taqqoslaganda, backend dasturlash tillarini tanlash ancha kengroq va siz foydalanish holati va muhitingizga qarab bitta yechim topishingiz mumkin.

#### Skriptlash tillari

Bajarilishidan oldin aniq kompilyatsiya qilishni talab qilmaydigan tillar skript tillari yoki sharhlangan tillar deb nomlanadi. Tarkib qilingan tillardan farqli o'laroq, ular ikkilik bajariladigan (binary executable ) ishlab chiqmaydi. Aksincha kod baholanadi va tezlikda ishlaydi. Ba'zida skript tillarini boshlash osonroq bo'ladi, chunki kodni kompilyator tomonidan talab qilinadigan tarzda yozishingiz shart emas. Ammo bu shuni anglatadiki, kompilyatsiya paytida aniqlangan xatolar faqat ish vaqti davomida aniqlanadi.

![backendlangs](/media/backend.jpg "foto: muzel")

> P.S: Dasturlashdagi atamalar sizga biroz tushunarsiz tuyulishi tabiiy. Ba'zi atamalarni o'zbek tilida tarjimasi yo'q yoki tushunarsiz bo'ladi. Tajribangiz oshishi bilan bular sizga tanish bo'lib qoladi, Xudo xohlasa.

##### Eng mashhur skript tillari:

* [Node.js](https://nodejs.org/en/) server tomonidan ishlaydigan JavaScript. U o'zining JavaScript xususiyatlarini to'plamini qo'llab-quvvatlaydi va fayl tizimi bilan ishlash kabi foydalanishni backend holatlarini qondirish uchun API to'plamini taqdim etadi. Node.jsni o'rganish juda yaxshi tanlovdir, chunki bitta tilni o'rganish bilan siz old va orqa tomondan ishlashingiz mumkin. Node.js [ekspress](https://expressjs.com/), [koa ](https://koajs.com/)yoki [LoopBack ](https://loopback.io/)kabi bir nechta mashhur freymvorklarga ega. 	
* [Python ](https://www.python.org/)- bu umumiy maqsadli dasturlash tili. Oddiy sintaksis va aniq konstruktsiyalar yangi boshlanuvchilar uchun o'rganishni juda osonlashtiradi. Python dasturlarni ishlab chiqishda keng qo'llaniladi, ammo u ilmiy izlanishlar va sun'iy intellekt bilan ishlashda katta tortishlarga ega bo'ldi. Hozirda ikkita asosiy versiya ishlatilmoqda: Python 2 va Python 3. Python-da ishlab chiqilgan mashhur loyihalardan biri bu [Django ](https://www.django-cms.org/en/)tarkibini boshqarish tizimi. [Flask ](https://flask.palletsprojects.com/en/1.1.x/)veb-ishlab chiqarish uchun mashhur mikro-freymvorkdir. •	
* [PHP ](https://www.php.net/)- veb-ilovalar uchun yana bir mashhur dasturlash tili. Tilning o'zi yangi boshlanuvchilar uchun past kirish to'sig'iga ega, ammo oraliq foydalanuvchilar uchun yanada rivojlangan xususiyatlarni taqdim etadi. PHP-da yaratilgan eng mashhur loyihalarning ba'zilari [WordPress ](https://wordpress.org/download/)va [Drupal ](https://www.drupal.org/)bo'lib, ular ilgari dunyoda eng ko'p ishlatiladigan kontentni boshqarish tizimi hisoblanadi. [Laravel](https://laravel.com/), [Symfony ](https://symfony.com/)va [CodeIgniter ](https://codeigniter.com/)taniqli freymvorklardir. 
* [Ruby ](https://www.ruby-lang.org/en/)- o'qish va yozish uchun oddiy va tabiiy bo'lishi uchun yaratilgan skript tili. Ruby uchun eng mashhur rivojlanish doirasi bu [Ruby on Rails](https://rubyonrails.org/). [Jekyll](https://jekyllrb.com/), mashhur statik veb-sayt yaratuvchisi Ruby-da qurilgan.

##### Kompilyatsiya qilingan tillar

Kompilyatsiya qilingan tillar yordamida yozilgan kodni bajarishdan oldin avval ikkilik faylga ( binary file) kompilyatsiya qilish kerak. Garchi buning uchun dasturchi tomonidan aniq qo'shimcha qadam qo'yishi kerak bo'lsa-da, qo'shimcha foyda keltiradi. Kompilyator (compiler) kodni mos kelmasligi uchun tahlil qilishi va yuzaga kelishi mumkin bo'lgan muammolar haqida sizga erta javob berishi mumkin. Ba'zi kompilyatorlar, shuningdek, natijaviy bytekodni ma'lum bir platforma uchun ishlashini ta'minlaydigan optimallashtirishlari mumkin. Kompilyatsiya qilingan tillar skript tillariga qaraganda yuqori kirish to'sig'i (barrier) ga ega bo'lishi mumkin, ammo ular qo'shimcha xavfsizlik choralari va tavsif kodi tufayli katta loyihalarda afzalroqdir.

* [Java ](https://www.java.com/en/)- bu Sun Microsystems tomonidan ishlab chiqilgan va hozirgi kunda Oracle tomonidan boshqariladigan yuqori darajadagi ob'ektga yo'naltirilgan dasturlash tili. Java har xil platformalar o'rtasida ko'chiriladigan qilib yaratilgan: manbalar Java baytekodiga kompilyatsiya qilingan, uni istalgan platforma uchun Java Virtual Machine-da ishlatish mumkin. Bu juda etuk til bo'lib, veb-ilovalarni ishlab chiqish uchun juda ko'p turli xil ramkalarga ega, eng mashhuri - [Spring](https://spring.io/). Bundan tashqari, Java-dan Android dasturlarini ishlab chiqish uchun foydalanish mumkin.
* [C# ](https://docs.microsoft.com/en-us/dotnet/csharp/)- bu Microsoft tomonidan ishlab chiqilgan yuqori darajadagi ob'ektga yo'naltirilgan dasturlash tili. Dastlab Windows-da ishlab chiqilgan bo'lib, endi nisbatan yangi [.NET Core](https://dotnet.microsoft.com/download) ish vaqtidan platformalar-aro dasturlarni yaratish uchun ishlatilishi mumkin. C# - dan foydalanib veb-dasturlarni yaratish uchun eng mashhur ramkalardan biri bu [ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/?view=aspnetcore-2.1). C# Microsoft-ning texnologiya to'plamini qo'llaydigan kompaniyalar orasida mashhur.
* [Go ](https://golang.org/)- bu Google tomonidan ishlab chiqilgan va tezda mashhurlikka erishgan nisbatan yosh til. U Java yoki C # ga qaraganda kamroq og'zaki bo'lishi uchun yaratilgan va sodda vositalarga asoslangan bo'lib, boshqa tillarda mavjud bo'lgan ba'zi murakkab konstruktsiyalarni o'zida jamlamaydi. Go juda tezkor, minimal xotira iziga ega va birinchi darajali moslashuvchan qo'llab-quvvatlovga ega, shuning uchun tez va kam resurs iste'moli muhim bo'lgan loyihalar uchun yaxshi nomzod. Go blockchainni rivojlantirishda katta mashhurlikka erishgan.
* [Kotlin ](https://kotlinlang.org/)- JetBrains tomonidan ishlab chiqilgan til va Java-ning yaqin raqobatchisi. Kotlin Java virtual mashinasida ishlaydi, ammo uni JavaScript-ga ham Kompilyatsiya qilish mumkin. Java-ga qaraganda kamroq og'zaki bo'lishi uchun yaratilgan, birinchi darajali funktsiyani qo'llab-quvvatlaydi va keng tarqalgan xatolarga yo'l qo'ymaslik uchun qo'shimcha xavfsizlik choralarini taklif qiladi. Java kabi, u Android dasturlarini ishlab chiqish uchun ham ishlatilishi mumkin.
* [Scala ](https://www.scala-lang.org/)- bu boshqa JVM asosidagi til va Java-ga alternativa. U yanada ixcham sintaksisga, qo'shimcha xavfsizlik xususiyatlariga ega va funktsional dasturlashdan juda ko'p foydalanadi.
* [Erlang ](https://www.erlang.org/)- mos kelishlik va yuqori imkoniyatlarga ega bo'lish uchun mo'ljallangan funktsional til. Erlang yuqori samaradorlik va miqyoslilik juda muhim bo'lgan dasturlarda mashhur. Ommaviy foydalanish holatlariga tasvir va signallarni qayta ishlash yoki katta hajmdagi ma'lumotlarni tahlil qilish kiradi.
* [Haskell ](https://www.haskell.org/)- kuchli yozish tizimi, aniq va ishonchli kod ishlab chiqarishga yordam beradigan dizayni uchun qadrlanadigan yana bir funktsional dasturlash tili. Funktsional til bo'lgani uchun, u ham samarali darajada ishlaydi va yaxshi ishlashga imkon beradi.

##### Ma'lumotlar bazalari

![db](/media/5de3ea6fa3e02f17cf246d201d8d67cb.png "foto: proglib")

Ko'pgina dasturlarning muhim qobiliyati foydalanuvchi ma'lumotlarini saqlashdir. Odatda bu ma'lumotlar bazasini boshqarish tizimlari (Database management systems) deb nomlangan maxsus dastur yordamida amalga oshiriladi. Ma'lumotlar bazasi ma'lumotlar omboriga kirishni ta'minlaydi, bu esa ilovalarga ma'lumotlarni saqlash, olish va yangilash imkonini beradi. Turli xil shakllar va hajmlar uchun optimallashtirilgan turli xil ma'lumotlar bazalari mavjud. ushbu qo'llanmada biz eng mashhur ikki turni ko'rib chiqamiz: aloqador va aloqador bo'lmagan. ( relatsional  va no-relatsional)

##### Relatsional

Relatsional ma'lumotlar bazalari ma'lumotlarni jadvallarda saqlaydi, unda satrlar yozuvlarni, ustunlar esa - kirish atributlarini aks ettiradi. Turli xil jadvallardagi satrlarni turli xil yozuvlar o'rtasidagi munosabatlarni ifodalash uchun tashqi tugmachalar yordamida bog'lash mumkin. Masalan, agar siz onlayn-do'kon qurayotgan bo'lsangiz, sizda "buyurtma raqami", "mijoz nomi" va "etkazib berish manzili" kabi ustunlarni o'z ichiga olgan jadval bo'lishi mumkin, bu yerda har bir satr alohida buyurtmani aks ettiradi.

Aksariyat aloqador ma'lumotlar bazalari ma'lumotlarni so'rash yoki o'zgartirish uchun Strukturalangan so'rovlar tili (SQL- Structured Query Language). Shu sababli, ular ko'pincha SQL ma'lumotlar bazalari deb nomlanadi.

###### Ommabop relatsion ma'lumotlar bazalari:

• [Oracle ma'lumotlar bazasi](https://www.oracle.com/database/) - bu Oracle tomonidan ishlab chiqilgan ma'lumotlar bazasi. Keng miqyosliligi va kuchli xususiyatlari tufayli, ko'pincha yirik korxonalar tomonidan foydalaniladi. U litsenziyali yuqori xarajatlar tufayli kichik va o'rta loyihalarda kamroq ishlatiladi. 

• [MySQL ](https://www.mysql.com/)- shved kompaniyasi MySQL AB tomonidan ishlab chiqilgan va hozirda Oracle-ga tegishli bo'lgan ochiq manbali bepul ma'lumotlar bazasi. MySQL ma'lumotlarni saqlash va boshqacha ishlatish uchun har bir jadval uchun turli xil saqlash motorlaridan foydalanishi mumkin. MySQL keng ko'lamli holatlarda qo'llaniladi, ammo veb-dasturlar uchun juda mashhur, ayniqsa LAMP (Linux, Apache, MySQL, PHP) deb nomlangan stekda. Bundan tashqari, keng miqyosli foydalanuvchilar uchun bir nechta pullik nashrlarni taklif etadi.

•[ SQL Server ](https://www.microsoft.com/en-us/sql-server)- shuningdek MSSQL deb nomlanadi, bu Microsoft tomonidan saqlanadigan ma'lumotlar bazasi. U turli xil ish yuklari va ma'lumotlar hajmini qayta ishlash uchun bir qator turli xil nashrlarga ega.

• [PostgreSQL](https://www.microsoft.com/en-us/sql-server) - bu dunyo bo'ylab ko'ngillilar jamoasi tomonidan yaratilgan bepul ochiq manbali ma'lumotlar bazasi. U boy xususiyatlar to'plamini taqdim etadi va katta hajmdagi ishlarni bajarishga qodir.

###### No-relatsional ma'mumotlar bazalari:

![dbase](/media/screenshot_4-4.jpg "foto: proglib")

Aloqasiz ma'lumotlar bazalari ma'lumotlarni jadvaldan tashqari boshqa modellarda saqlaydi. Foydalanish holatlariga qarab siz tanlashingiz mumkin bo'lgan turli xil modellar mavjud, masalan, kalit qiymat juftligini, hujjatlarni, grafik aloqalarni yoki vaqt seriyasini saqlash. Garchi no-relatsional ma'lumotlar bazalari bir muncha vaqt bo'lgan bo'lsa-da, yaqinda ular sodda dizayni va masshtablashning osonlashishi tufayli ommalashdi.

No-relatsional ma'lumotlar bazalari, shuningdek, NoSQL ma'lumotlar bazalari deb ataladi, chunki ularning ko'plari SQL o'rniga o'z so'rovlarini ishlatadilar.

• [MongoDB ](https://www.mongodb.com/)- bu JSON-ga o'xshash ob'ektlarni saqlaydigan bepul ochiq manbali hujjatlar bazasi. Siz ushbu ob'ektlarni saqlashingiz va olishingiz va ularni ilovangizdagi ob'ektlarga xaritalashingiz mumkin. Bundan tashqari, odatiy so'rov va yig'ish qobiliyatiga ega. MongoDB ma'lumotlar barqarorligi asosiy tashvish tug'dirmaydigan dasturlar uchun yaxshi nomzod.

 • [Redis ](https://redis.io/)- tez-tez keshlangan ma'lumotlarni vaqtincha saqlash va xabarlarni uzatish uchun ishlatiladigan xotiradagi kalit qiymatidagi ma'lumotlar bazasidir. Bunday ma'lumotlarni majburiy ravishda saqlash kerak emasligi sababli, ishlashni oshirish uchun ma'lumotlarni diskka saqlash o'chirib qo'yilishi yoki kechiktirilishi mumkin. Redis turli xil qiymatlarni, masalan, satrlar, raqamlar, ro'yxatlar, xaritalar va boshqalarni saqlashi mumkin

• [Elastic Search ](https://www.elastic.co/)- bu ochiq manbali matn qidirish va tahlil qilish mexanizmi. Bu sizga matnli hujjatlarni saqlashga imkon beradi va qidiriladigan matn indeksini yaratadi. Elastik Qidiruv odatda jurnalni tahlil qilish uchun (ayniqsa ELK stack qismi sifatida) va tekstli hujjatlarni bepul qidirishda ishlatiladi.

##### Xabarlashuv

Ba'zan server tomonlari fonda bajarilishi kerak bo'lgan ishlarni boshlashi kerak. Masalan, biznes-hisobotni so'rash uzoq vaqt davom etadigan jarayonni boshlashi mumkin, bu hisobotni yaratadi va foydalanuvchiga elektron pochta orqali, uni kutib o'tirmasdan yuboradi. Buning uchun biz boshqa tarkibiy qismga xabar yuborishimiz va uning muvaffaqiyatli bajarilganligiga ishonch hosil qilishimiz kerak. Agar ish bajarilmasa, uni qayta boshlash kerak. Bunday funktsiyani ta'minlaydigan dastur xabarlar brokeri deb nomlanadi. 

 **Ikki mashhur xabarlar vositachilari:**

• [RabbitMQ ](https://www.rabbitmq.com/)- bu xabarlarni etkazib berishning turli modellari va yo'naltirish qoidalarini qo'llab-quvvatlaydigan an'anaviy xabarlar vositachisi. Xabar iste'molchiga etkazilishi va qayta ishlanishiga kafolat beradi. Muvaffaqiyatsiz xabarlarni o'lik harflar navbatida saqlash mumkin. RabbitMQ standart [AMPQ protokoli](https://www.amqp.org/) orqali ishlaydi, uni boshqa xabar brokerlari va mijozlar kutubxonalari ham qo'llab-quvvatlaydi. 

• [Apache Kafka](https://kafka.apache.org/) - bu xabarlar vositachisi sifatida ishlatilishi mumkin bo'lgan oqimni qayta ishlaydigan dvigatellar. Oddiy xabarlar vositachisi funktsiyalarining aksariyat qismini taqdim etishdan tashqari, u tarixdagi xabarlarni qayta ishlash imkoniyati kabi rivojlangan xususiyatlarni ham taklif etadi. Bundan tashqari, u yuqori hajmdagi xabarlarni qayta ishlashga imkon beradi.

![done](/media/undraw_done_a34v.png "foto: undraw")

Agar siz ushbu ikkita postlar bilan tanishib chiqqan bo'lsangiz, sizda frontend va backend texnologiyalari haqida yetarlicha ma'lumot bo'lishi kerak. Qaror qabul qilishdan oldin va qaysi texnologiyani tanlashdan oldin blogdagi havolalarni ko'rib chiqishingizni maslahat beraman.

\    \*                \*               *

 Keyingi postda har bir dasturchi bilishi kerak bo'lgan vositalarni ko'rib chiqamiz.
\
*manba: https://medium.com/devtrailsio/beginners-web-development-guide-part-2-backend-fd466212dbfc dan tarjima qilindi.*