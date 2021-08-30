Kitoblarda, jurnallarda ko'pincha olim va ziyoli odamlarning iqtiboslarini keltirishadi:

> <q>Muhandis - qurilmaning ishlashini tushuntirib bera oladigan, lekin nima uchun ishlamayotganini tushuntirolmaydigan kishi.</q>
> 
> M. Tetcher.

HTML da 2ta iqtibos teglari mavjud:

1. `<q>..</q>` - Qisqa bo'lgan iqtiboslar uchun
2. `<blockquote>..</blockquote>` - Uzun iqtiboslar uchun

### 1. Qisqa iqtibos

`<q> .. </q>` tegi orasidagi matin odatta *"* - qo'shtirnoq belgisi bilan o'raladi.

:::main{#warn}
`q` tegi `p` tegidan farqli o'laroq, matinni yangi qatordan boshlamaydi, aksincha uni davom etadi.
:::

~~~html
<q>Agar yolg'onni yetarlicha uzoq muddat, baland ovozda va tez-tez gapirilsa, odamlar ishonishni boshlaydi.</q>

Adolf Gitler.
~~~

Lekin bizda muammo! Muallif berilgan iqtibos bilan bir qatorda, bizga esa yangi qatordan kerak:

~~~html
<q>Agar yolg'onni yetarlicha uzoq muddat, baland ovozda va tez-tez gapirilsa, odamlar ishonishni boshlaydi.</q>

<br />
Adolf Gitler.
~~~

### 2. Uzun iqtibos

Aynan `q` tegi qisqa iqtiboslar uchun mo'ljallanganligi sababli yangi qatorga o'tmaydi. Undan farqli `blockquote` yangi qatorga o'tadi (xuddi `p` tegi kabi), va qo'shimcha chap va o'ng tarafidan boshliq qo'shib, tepa va past qismidan ozgina masofa ochadi.

~~~html
<blockquote>
    <p>Agar yolg'onni yetarlicha uzoq muddat, baland ovozda va tez-tez gapirilsa, odamlar ishonishni boshlaydi.</p>
    <i>Adolf Gitler.</i>
</blockquote>
~~~

Payqang, `blockquote` ichidan `p` tegini qo'lladik, lekin `q` tegida bunday qilish ma'n etilgan. Sababi blockquote bu *block* element, `q` esa *inline*. Buni keyingi darsga qoldiramiz.

### Qo'llanilishi

Kelajadkda yangiliklar sayti ([kun.uz](#), [daryo.uz](#) va h.k) yoki shaxsiy blog yasash uchun buyurtma olganingizda, eng ko'p ishlatadigani shulardir.

:::main{#info}
Asosan *yozish* bilan bog'liq saytlarda ishlatiladi.
:::
