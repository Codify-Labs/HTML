## Muammo
Birinchi saytingizni siz o'tgan darsda yaratishga ulgurdingiz. Agar siz o'tgan darsdagi [ikkinchi](#) mashqni ishlagan bolsangiz, mini-brauzerda mana shunday natijani kordingiz:

> Mening Ismim ____, familyam ____ yoshim ____ da. Dasturlashni o'rganishimdan maqsad...

Xech qanday abzaslar yo'q, qanchama urinmang yangi qatorga o'tkaza olmaysiz. Bunig sababi siz yozgan matin bu to'liq HTML emas. HTML da har-bir matin, va har bir ma'lumotni ekranga ko'rsatishda o'zining maxsus sintaksisi mavjud (Xuddi *Microsoft Word*da yozganda oddiy matinni sarlavhaga aylantirsh uchun xajmini va qoraligini yiriklashtirganimizdek). 

Agar siz o'tgan mashqni bajarmagan bo'lsangiz mana shu mattinni ozingiz sinab ko'ring:

~~~html
Why do we use it?
It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout.

Where does it come from?
Contrary to popular belief, Lorem Ipsum is not simply random text. It has roots in a piece of classical Latin literature from 45 BC, making it over 2000 years old. 
~~~

[lipsum.com](https://www.lipsum.com/) saytidan olindi.

Natija o'sha-o'sha ierarxiyasiz.

## HTML - Teg

HTML da xar bir ma'lumotni ekranga to'g'ri ko'rsatish uchun *teglar* ishlatilinadi. HTML ko’p turdagi teglardan tashkiltopgan, va har-bir element uchun alohida maxsus teg mavjud.

HTML teg 3 qismdan iborat *ochilish*, *kontent*, *yopish*.

#### 1. Ochish tegi

Ochish tegi `<` va `>` burchakli qavslari orasida o'z nomi yozilib ochiladi: `<Teg nomi>`

#### 2. Yopish tegi

Ba’zi teglarni inobatga olmaganda, hamma teglar o’zining yopiluvchi teglari ham bo’lishini talab qiladi, va u shu ko'rinishda bo'ladi: `</Teg nomi>` - */* ishlatiladi.

Ochis tegidan farqi `<`dan keyin */* qo'shiladi.

Va ochilish tegi bilan birlashib bir funksional yaratadi, `<Teg>...</Teg>`. Orasiga qo'yilgan matin, shu *teg* qanday funsiyani amalga oshirsa shunga aylanadi.

#### 3. Kontent

Kontent ochish va yopish orasidagi matin yoki xohalagan turdagi ma'lumot: `<Teg> Kontent </Teg>`.

Demakki *HTML teg* mana shunday ko'rinishda bo'lar ekan:

![TAG_EXPLANATION](https://i.ibb.co/DtDbmwn/Group-7.png)

:::info
*Teg* joyida HTML da mavjud maxsus so'zlar uning o'rniga qo'yiladi va kerakli natijani olamiz.
:::

Misol:

Masalan HTML da matinni sarlavhaga aylantrish uchun `h1` - nomli teg orasiga qo'yib qo'llaniladi.

~~~html
<h1>Men Sarlavhaga aylanaman</h1>
~~~

Shu kodni sinab ko'ring. Xo'sh natija sizni lol qoldirdimi? Unchalik qiyin emas a?

Bo'ldi shu, HTML bu teglar xolos! Juda oson..

Oddiy matin yaratmoqchimisiz? Unda `p` nomli tegni ishlating:

~~~html
<h1>Men Sarlavhaga aylanaman</h1>

<p>Men Oddiy Matinman</p>
<p>Menham Oddiy Matinman</p>
~~~

Natija esa biz kutgandek. Ajoyib.

Keyingi bosqich kerakli teglarning hammasini o'rganib (Rasm tegi, Jadval tegi va h.k), amalda sinab, haqiqiy loyihada ishlab o'rganish.
