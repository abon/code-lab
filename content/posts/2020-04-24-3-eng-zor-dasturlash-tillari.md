---
template: post
title: '3 Eng Zo''r Dasturlash Tillari '
slug: top-prog-langs
draft: false
date: 2020-04-24T20:21:22.164Z
description: >-
  Dasturlashni boshlovchilar uchun 3 nafar eng qulay va talabgir bo'lgan
  dasturlash tillari
category: Programming Languages
tags:
  - Programming Languages Advice
---
![top prog langs](/media/1.jpeg "foto: medium")

Dastlabki o'rganuvchi dasturchi sifatida o'rganish uchun eng yaxshi uchta dasturlash tillarini ko'rib chiqish uchun yaxshi vaqt. Faoliyatim davomida men bir nechta dasturlash tillaridan foydalanganman va ularni ko'p o'zgartirganman. 

📊 **Google**ning tendentsiyalari asosidagi eng zo'r dasturlash tillari bo'yicha ma'lumoti boshlovchi dasturchilar uchun ayni muddao bo'ladi.

![google pic](/media/2.png "foto: google")

**Bu to'g'ri! 🔥**

Bu **Python**, **JavaScript** va **Java** bir necha tadqiqotlar davomida eng yaxshi dasturlash tillari sifatida tanlangan. Ushbu blog postida biz ushbu tillarning asosiy xususiyatlarini va bir-birlaridan qanday farq qilishlarini bilib olamiz.

![python](/media/3.png "foto: medium")

**[Python ](https://www.python.org/)**har doim eng sevimli dasturlash tillaridan biridir. Uni ishlatish juda oddiy va har qanday chalkashliklardan xoli.

>  AQShda Python dasturchisining [o'rtacha ish haqi ](https://www.indeed.com/salaries/python-developer-Salaries)**yiliga** $118,626 tashkil etadi.

[2019 yilgi Stackoverflow tadqiqotida](https://insights.stackoverflow.com/survey/2019#most-loved-dreaded-and-wanted) Python ishlab chiquvchilar tomonidan yilning eng ko'p tilga olinadigan dasturlash tili sifatida joy oldi. Bu meni ajablantirmaydi, chunki Python dasturchilar bilan do'stona til sifatida tanilgan.

![python](/media/4.png "foto: medium")

#### 👨🏻‍💻Python kodi qanday ko'rinishga ega

```
num = int(input("Sonni juft yoki toq ekanini bilish uchun kiriting: "))
if (num % 2) == 0:
   print("{0}  Juft".format(num))
else:
   print("{0} Toq".format(num))
```

Python uchun yangi bo'lganlar uchun ushbu sintaksis boshqa dasturlash tillaridan farqli ravishda ko'rinishini ko'rasiz. Hech qanday jingalak qavslar, sinflar yo'q va ommaviy / xususiy modifikatorlar mavjud emas. Bu juda sodda va tartibli. Bu Python-ning ishlab chiquvchilarga juda yoqadigan sabablaridan biridir. Endi yuqorida ko'rsatilgan dasturning natijalarini ko'rib chiqaylik.

```
Sonni juft yoki toq ekanini bilish uchun kiriting: 56
56
56 Juft 
```

#### 💁🏻‍♂️ Nima uchun Python?

Python nima uchun bugungi kunda eng yaxshi dasturlash tillaridan biri sifatida ro'yxatga olinganligi haqida qisqacha ma'lumot:

* Foydalanish uchun oddiy
* Kodda chalkashliklar yo'q
* Dasturlashni boshlayotganlar uchun o'rganish oson
* Mashinalarni o'rganish, AI loyihalari va tadqiqotlar uchun eng mos
* Ob'ektga yo'naltirilgan paradigmalarga amal qiladi
* Frontend va Backend dasturlarni yaratish uchun foydalanish mumkin
* Ma'lumot olimlari (data scientist) tomonidan keng qo'llaniladi
* Katta Python jamiyati

#### 🙅‍♂️ Nega Python emas?

Python shu qadar rivojlantiruvchi va ommabop, lekin har doim har bir dasturlash tilida ba'zi kamchiliklar mavjud. Python nima uchun yaxshi tanlov bo'lmasligi mumkinligi ro'yxati:

* **📱 Mobil rivojlanish uchun mos emas** - Python mobil rivojlantirish uchun deyarli ishlatilmaydi, chunki React Native, Flutter va Swift va Java kabi mahalliy tillar mavjud. Shunday qilib, Python-da kodlangan mobil dasturlarni topa olmaysiz.
* 😓 **Boshqa dasturlash tillarini o'rganish qiyin** - agar Python siz o'rganadigan birinchi til bo'lsa, unda siz uning soddaligiga oshiq bo'lishingiz mumkin va natijada boshqa dasturlash tillarini o'rganish qiyinlashadi. Python-dan ko'chib o'tishda Java kabi boshqa dasturlash tillari murakkab ko'rinishi mumkin.
* 📈 **Keng miqyosli dasturiy ta'minotni ishlab chiqishda foydalanilmaydi** - Python yirik kompaniyalarda korxona dasturiy ta'minotini ishlab chiqish uchun ko'p ishlatilmaydi. Java va JavaScript kabi tillar taqqoslashda ko'proq ishlatiladi. Python ish vaqtida sekinroq va ma'lumotlar bazasiga kirishda cheklovlarga ega. Python ma'lumotlar bazasiga kirish qatlami JDBC yoki ODBC kabi yaxshi emas va keng ko'lamli dasturlar uchun mos emas.

# Java

![java](/media/5.jpeg "foto: medium")

Keyingi eng yaxshi dasturlash tili - bu **[Java](https://www.java.com/en/)**. Java - eng ko'p ishlatiladigan dasturlash tillaridan biri bo'lib, u 2020 yilda o'rganish uchun mukammal til bo'ladi.

> AQShda Java ishlab chiqaruvchisining o'rtacha ish haqi **yiliga** $103,464 tashkil etadi.

Karyeramni boshida men korxonalar dasturiy ta'minoti uchun juda ko'p Java kodini yozdim. Java keng ko'lamli dasturiy ilovalarda keng qo'llaniladi.

#### Keling, ba'zi Java kodini ko'rib chiqaylik

Endi Python-dan Java-da foydalanib, oldin yozgan dasturimizni yozaylik. Dastur foydalanuvchining kirishini oladi va raqam top yoki juftligini tekshiradi.

```
import java.util.Scanner;
public class ToqJuft {
    public static void main(String[] args) {
        Scanner reader = new Scanner(System.in);
        System.out.print("Raqam kiriting: ");
        int num = reader.nextInt();
        if(num % 2 == 0)
            System.out.println(num + " soni Juft");
        else
            System.out.println(num + " soni Toq");
    }
}
```

E'tibor bering, sintaksis Python-dan mutlaqo farq qiladi. Bu erda biz sinf, ommaviy / shaxsiy kirish, skaner va boshqalar kabi tushunchalarni taqdim etdik. Java dasturlari Python kabi tillarga qaraganda ancha strukturaga boy tuzilgan. Java-dagi hamma narsa sinf yoki interfeys ichida bo'lishi kerak.

#### ️️️️💁🏻‍♂️ ️Nima uchun Java?️

Nima uchun Java-ni o'rganishingiz kerakligi haqida qisqacha ma'lumot:

* **👨🏻‍💻 Java dasturiy ta'minot dasturlarida qo'llaniladi** - Java-ni o'rganishning asosiy sabablaridan biri shundaki, u keng ko'lamli dasturlarni yaratish uchun dunyoning ko'plab texnologik kompaniyalarida qo'llaniladi. Uber, AirBnb, Twitter va boshqa ko'plab yirik kompaniyalar o'zlarining texnik stakalarida Java-dan foydalanadilar. Bu shuni anglatadiki, Java dasturchisi sifatida ish topish nisbatan oson.
* 💻 **Performance** - Java-da yozilgan ilovalar ishlash uchun optimallashtirilgan va dinamik yozilgan tillarga qaraganda tezroq ishlaydi. JVM-lar zamonaviylashtirilgan va juda yaxshi bajarilgan, bu katta ilovalar uchun juda mos keladi.
* 📲 **Android Development** - Java mahalliy Android ilovalarini yaratishda ishlatiladi. Agar siz mahalliy Android-dasturlarni yaratishga yo'naltirilgan mobil dasturchi bo'lishni istasangiz, unda Java-ni o'rganish juda yaxshi yo'l
* 👨🏽‍🤝‍👨🏽 **Katta hamjamiyat** - Java o'n yildan ortiq vaqtdan beri ommabop dasturlash tili bo'lib kelmoqda va katta jamoatchilik tomonidan qo'llab-quvvatlanmoqda. Java-ni o'rganishni boshlaganingizda, siz o'qishda yordam beradigan ko'plab manbalar, forumlar va kitoblarga duch kelasiz.
* 🛠 **Platforma va Asboblar** - Java ekotizimi yillar davomida rivojlanib bordi va Java-da [IntelliJ](https://www.jetbrains.com/idea/), [Eclipse ](https://www.eclipse.org/)va boshqalar kabi rivojlanishni qo'llab-quvvatlaydigan turli xil ajoyib vositalar va IDE mavjud.

#### 🙅🏻‍♂️ Nima uchun Java emas?

Xo'sh, nima uchun Java emasligini bilib olaylik:

* **⛓ Verbose Code** - Java kod juda verbaldir va yangi boshlovchi dasturchini chalkashtirib yuborishga moyildir. Bu shuni anglatadiki, kod ba'zi ishlab chiqaruvchilarni asabiylashtirishi mumkin bo'lgan juda ko'p takrorlanadigan elementlar bilan ta'minlangan. Java-ning ko'p qirrali tabiatini tushunish uchun siz yuqoridagi misolimizdan kod parchalarini taqqoslashingiz mumkin.
* ❗ **Eski til** - Yangi yoshdagi dasturchilar va startaplar Java-ga boshqa alternativalarni tanlashga moyildirlar. Buning sababi eski va ular o'rniga yangi, zamonaviy dasturlash tilini o'rganishni afzal ko'rishadi. Agar siz boshlang'ich dasturlar va zamonaviy texnologiyalar uchun ishlashni rejalashtirmoqchi bo'lsangiz, sizga mos keladigan boshqa dasturlash tilini o'rganishni o'ylab ko'rishingiz mumkin.

# JavaScript

![js](/media/6.png "foto: medium")

Keyinchalik 2020 yilda o'rganish uchun dasturlashning keyingi eng yaxshi tili bu mening eng yoqtirgan [JavaScript ](https://www.w3schools.com/js/)tilim.

> AQShda JavaScript dasturchilarining o'rtacha ish haqi **yiliga** @113,615 tashkil etadi

📈 [StackOverflow tomonidan o'tkazilgan so'rovnomada](https://insights.stackoverflow.com/survey/2019#technology) ettinchi yil ketma-ket JavaScript eng mashhur dasturlash tili sifatida birinchi o'rinni egallab turibdi.

![js](/media/7.png "foto: medium")

#### JavaScript Kodi

Quyidagi kod parchasida biz "buJuft" funktsiyasini yozdik, u raqamni oladi va u juft yoki toq ekanligini tekshiradi. Konsolga javob yozish uchun console.log ishlatiladi. Bu oxirgi foydalanuvchiga ko'rsatilmaydi. Konsol jurnalini yaratish ishlab chiqaruvchilar uchun sinov va nosozliklarni tuzatish uchun foydalidir.

```
function buJuft(num) {
    if (num % 2 === 0) {
        console.log(num + " soni Juft");
        return true;
    } else {
        console.log(num + " soni Toq");
        return false;
    }
}
```

#### 💁🏻‍♂️ Nima uchun JavaScript?

Sizda JavaScript-ni 2020 yilda o'rganishingiz kerak bo'lgan ko'plab sabablar mavjud. Quyida ulardan ba'zilari keltirilgan:

* **🔥 U hamma joyda ishlatiladi** - bugungi kunda deyarli barcha zamonaviy old ilovalar JavaScript-da yaratilgan. Agar siz zamonaviy frontend ilovasida ishlayotgan bo'lsangiz, JavaScript-ni chetlab o'tishingiz yoki e'tiborsiz qoldirishingiz mumkin emas.
* 💡 **Zamonaviy freymvorklar juda ko'p** - Bugungi kunda tashqi ko'rinishni rivojlantirishni qo'llab-quvvatlash uchun JavaScript-da yozilgan ko'plab yuqori sifatli freymvorklarva kutubxonalar mavjud. Zamonaviy frontend dasturlarini yaratish uchun [React](https://reactjs.org/), [Vue](https://vuejs.org/), [Angular](https://angular.io/), [React Native](https://facebook.github.io/react-native/) va boshqa freymvorklar keng qo'llaniladi.
* ✅ **Dasturchilarga do'stona va oson o'rganish** - JavaScript-ga kiradigan dasturchilar uchun do'stona til. Buning sababi bir nechta omillar bo'lishi mumkin. Tilning o'zi ishlab chiquvchilarni o'ziga jalb qiladi va qo'shimcha ravishda ishlab chiquvchilar tajribasini rivojlanishni qo'llab-quvvatlash uchun mavjud bo'lgan zamonaviy ekotizimlar bilan boyitadi.
* 🏙 **Ish imkoniyatlari** - JavaScript ishlab chiquvchilariga jahon bozorida talab katta. Google, Facebook, Uber va boshqalar singari Fortune 500 kompaniyalari JavaScript-ni rivojlantirishga katta miqdordagi sarmoyalarni jalb qiladilar va shu bilan JavaScript bozorida ko'plab ish imkoniyatlarini yaratadilar.
* ✌🏻**Ikkala Frontend va Backend Development** - Shunisi e'tiborga loyiqki, JavaScript-ning tashqi ko'rinishini yaratish sahnasida hukmronlik qilsa-da, lekin Node.js kabi ramkadan foydalanib, backendni yaratishda juda ko'p ishlatiladi. Bu shuni anglatadiki, zamonaviy JavaScript bilan siz frontend va backend fonda ishlab chiquvchi bo'lishingiz mumkin.
* 🚅 **Tezlik** - JavaScript dasturlari juda tez ishlaydi, chunki barcha kodlar mijoz (client) tomonida ishlaydi.
* #### 🙅🏻‍♂️ Nima uchun JavaScript emas?

  * 😓**Tez o'zgaradi -** Bu sizning nuqtai nazaringizga qarab kamchiligi yoki yutug'i deb hisoblanishi mumkin. JavaScript va uning asoslari jadal rivojlanmoqda va bugungi kunda JavaScript uch yil avvalgidan farq qiladi. Doimiy o'zgarish shundan dalolat beradiki, unda ko'p sonli kuchlar va jamoatchilik ishtirok etmoqda. Ammo bu bilan davom ettirish uchun qo'rqitish ham mumkin.
  * 🔐 **Xavfsizlik muammolari -** JavaScript kodi mijoz tomonidan bajariladi va odatda kod ochiladi. Shunday qilib, agar ishlab chiqish jarayonida eng yaxshi amaliyotlar qo'llanilmasa, bu ba'zi xavfsizlik buzilishlariga olib kelishi mumkin.

![done](/media/undraw_done_a34v.png "undraw")

###### ☘ Agar siz ushbu blog postdan foyda olgan bo'lsangiz, iltimos, ushbu post do'stlaringiz bilan baham ko'ring.

🔖 *Post [ushbu havoladan ](https://medium.com/@codewithmosh/top-3-programming-languages-to-learn-in-2020-cb3c53d32ec9)tarjima qilindi.*