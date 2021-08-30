Sayt yaratganda 10000+ qator HTML kod yozishga tog'ri keladi.

Yaxshi sayt o'zida kamida 3 qismdan iborat bo'ladi:

*Header*, *Body*, *Footer* qismlari (ingl: Bosh, Ta'na va Osti qismlar).

Header qismda *Menu* yoki *Logo* bo'lishi mumkun, *Body* qismida asosiy ma'lumotlar va *Footer* qismida yakunlash, telefon raqamlar va sayt egasi haqida ma'lumotlar berilishi mumkun.

Asosiy qismlar yana parchalarga ajratiladi, Header 2 qismga ajraldi: Menu va Logo, balkim yana qismlar qo'shilar! Body ham bir nechta qismlardan iborat bo'lishi mumkun, Footer 3 qismga ajraldi: Yakunlash so'zi, Bog'lanish qismi, kompaniya xaqida ozgina ma'lumot.

Qisqasi sayt tuzulmasi deyarli barchasi shu ko'rinishga keladi:

![WEBSITE_LAYOUT](https://i.ibb.co/dtM3MXQ/Group-17.png)

HTML teglar bilan:

~~~html
<header>
<logo></logo>
<menu></menu>
</header>

<body>
<h1>Biz dunyodagi #1 raqamli kompaniya</h1>
</body>

<footer>
<p>Sayt haqida</p>
<p>Ishlash vaqti: 7:00 - 18:00</p>
<p>Kompaniya haqida...</p>
</footer>
~~~

Aynan shuni daraxtga o'xshab shohalashni HTML da *Parent - Child Relation* deyiladi, o'bekcha Ota-Ona va Farzandlar bog'liqligi.

Bosh qismida Ota-Ona bu:

`<header></header>`

Farzandlari:

1. `<logo></logo>`
2. `<menu></menu>`

:::main{#success}
Bitta teg o'z ichiga olgan boshqa teglar, *farzandlari* deyiladi, o'zi esa *OTA-ONA*
:::

`<logo>` va `<menu>` teglari bir birlari bilan teng qatorda joylashganlar *siblings*, ya'ni *aka-ukalar* xisoblanadi.

~~~html
<ota-ona>
<farzand-1></farzand-1>
<farzand-2></farzand-2>
</ota-ona>
~~~

`<farzand-1>` va `<farzand-2>` AKA-UKALAR (*siblings*).

:::main{#warn}
Tepadagi teglar HTML da *mavjud* emas, shunchaki namoyish uchun.
:::

Kodni tushunarli bo'lishi uchun `farzand` bo'lgan teglarni chap tarafidan 4 oraliq masofa tashash bilan yozish o'rinli bo'ladi:

~~~html
<ota-ona>
    <farzand-1></farzand-1>
    <farzand-2></farzand-2>
</ota-ona>
~~~

:::main{#info}
Klaviaturada *Tab* tugmasini bosish kifoya.
:::
