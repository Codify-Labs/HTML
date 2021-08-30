### Paragraflar yaratish

Paragraf yaratishni yuzaki [ko'rib otkandik](#), bugun mavzuni chuqurroq ko'rib chiqamiz.

Paragraf elementi veb-sahifalarda matnni ekranga, abzaslar bilan, ko'rsatish uchun ishlatiladi.

:::main{#info}
`<p>..</p>` Teglari matinni boshqa matinlarga qo'shmasdan, yangi qatordan, yuqori va pastki tarafidan bo'sh joy hosil qiladi.
:::

~~~html
Lorem ipsum dolor sit amet

<p>Lorem ipsum dolor sit amet</p>
~~~

Mana shundan farqli o'laroq, `<p>` matinni inson o'qishi mumkin bo'lgan shaklga keltiradi:

~~~html
Lorem ipsum dolor sit amet

Lorem ipsum dolor sit amet
~~~

### Matindagi bo'shliqlarni saqlab qolish

Odatta ko'plab *brauzerlar* paragraf ichidagi bo'shliqlarni (xat boshini) o'chirib tashlaydi.

~~~html
<p>
    Lorem ipsum dolor sit amet

    Lorem ipsum dolor sit amet
    Lorem ipsum dolor sit amet
<p>
~~~

Va xattoki matin ichidagi 2 va undan ko'p yaratilgan oraliqlarini:

~~~html
<p>
    Lorem       ipsum     dolor sit   amet
<p>
~~~

:::main{#warn}
Tepadagi berilayotkan kodlarning hammasini, o'ng tarafdagi *redaktorimizda* yozib, amalda sinab, ko'rib boring!
:::

Bu albatta saytga kirgan o'quvchiga noqulaylik va tushunarsiz bir xolatni keltirib chiqaradi.

Baxtimizga HTML da *xat boshi* va matinlarning orasiga chiziq tortish uchun maxsus teglar bor: `<br />` va `<hr />`.

#### Xat boshi

Tepada ko'rib o'tganimizdek `p` tegi orasidagi matinni boshqa matindan alohida qilib ko'rsatadi.

Shundan foydalanib yangi qator uchun bir nechta `p` teglarini xat boshi yaratish uchun ishlatsak bo'ladi:

~~~html
<p>100 gramm</p> 
<p>asal yig‘ish uchun asalari 46 ming km masofani uchib o‘tadi.</p> 
<p>Bu butun yer sharini ekvator bo‘ylab kezib chiqishdir.</p>
~~~

Lekin muammo shundaki biz bir to'liq bo'lgan matinni kichik-kichik parchalarga bo'lib tashladik.

Agar siz yangi paragrafni boshlamasdan satr uzilishini xohlasangiz, `<br />` dan foydalaning:

~~~html
<p>
    100 gramm asal 
    <br />
    yig‘ish uchun asalari 46 ming km masofani uchib o‘tadi. 
    <br />
    Bu butun yer sharini ekvator bo‘ylab kezib chiqishdir.
</p>
~~~

#### Chiziq tortish

Matin ichidan chiziq tortish uchun `<hr />` - ni ishlating:

~~~html
<p>
    Venera sayyoralar ichida, soat mili bo'yicha xarakatlanuvchi yagona sayyora.
    <hr />
    Yupiter, quyosh sistemasidagi, eng katta sayyora
</p>
~~~

#### Bo'shliq yaratish

Bo'shliq yaratish uchun xozircha HTML da xech qanday teg mavjud emas.

Lekin mavjud bo'lgan echim bu [HTML - Belgilardagi](#) `&nbsp;` belgisi (Oldimizdagi darsdan).

~~~html
<p>Lorem &nbsp;&nbsp;&nbsp; ipsum dolor sit amet</p>

<!-- Bundan farqli -->
<p>Lorem       ipsum dolor sit amet</p>
~~~

Ajoyib!

### O'z-o'zidan yopiluvchilar

*Self-closing* teglar (ingl.: O'z-o'zini yopuvchilar) bu odatiy teglardan, *ochilish*, *yopilish* va orasida matn yoki ma'lumot bo'lishi, olaroq bunday teglarda *yopish* va orasiga ma'lumot kirgizish shart emas, chunki bunga muxtoj emas. Aynan `<br />` va `<hr />` teglari *self-closing* teglaridan:

![SELF_CLOSING](https://i.ibb.co/vPxmySk/Group-8.png)

Qo'shimcha `<meta />`, `<link />`, `<input />`, `<img />`, `<embed />` va h.k. mavjud, va biz ularning barchasini kelgusi darslarda o'rganamiz.

:::main{#info}
##### 📌 Eslab qoling

Self-closing teglar `<teg-nomi />` shaklida bo'ladi.

Strukturasi:

`<` + `teg-nomi` + `/` + `>`
:::
