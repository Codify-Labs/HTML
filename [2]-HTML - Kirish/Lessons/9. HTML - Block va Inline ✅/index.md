### Mustail va Cheklangan

O'tkan darsdagi misolda biz `blockquote` tegi ichidan `p` tegini qo'lladik, sababi bu *block* element, ya'ni teg *mustaqildir*. `q` esa *inline* ya'ni *cheklangan*.

Va, agar teg *mustaqil* bo'lsa ichidan xohlagan tegni joylasak bo'ladi. Lekin *cheklanganda* bunday qilish ma'n etiladi!

#### Mustaqil teglar (*block*)

`<h1>`, `<h2>` ... `<h6>`, `<p>`, `<blockquote>`. (Biz o'tganlardan)

- Mustaqil teglar har doim yangi satrdan boshlanadi.
- Mustaqil teglar har doim to'liq *englikni* (width) egallaydi.
- Mustaqil teglar tepa va pastdan masofa ochadi.

#### Cheklangan teglar (*inline*)

Cheklanganlar teglar:

`<i>`, `<em>`, `<b>` ... , `<q>`

- Cheklangan teglar yangi qatordan <strong>boshlanmaydi</strong>!
- Cheklangan teglar faqat kerak kenglikni oladi, va agar ichidagi matin kichkina bo'lsa shu enlikni oladi xolos.
- Ko'pincha mustaqil teglarning ichida qo'llaniladi.

![BLOCK_AND_INLINE](https://i.ibb.co/QNsnzQF/Group-10-1.png)

Shu sababdan, agar biz bir nechta mustaqil (block) bo'lgan `p` teglarini ketma-ketlikda joylasak xar biri yangi qatordan boshlanadi. Undan farqli o'laroq, *cheklangan* teglarni ketma-ketlikda joylsak xammasi bir qatordan joy oladi:

~~~html
<!-- Mustaqil -->
<p>Lorem</p>
<p>ipsum</p>
<p>dolor</p>

<hr />

<!-- Cheklangan -->
<i>Lorem</i>
<em>ipsum</em>
<mark>dolor</mark>
~~~

Mustaqillarning hammasi alohida-alohida, ammo lekin cheklanganlar bir qatorda - (*Lorem ipsun dolor*).
