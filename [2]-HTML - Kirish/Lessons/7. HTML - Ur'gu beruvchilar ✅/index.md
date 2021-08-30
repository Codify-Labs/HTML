HTML da *paragraf* ichidagi maxsus so'zlarni ajratib ko'rsatish uchun alohida teglar mavjud.

> <b>Qalin</b> so'z
>
> <i>Kursivlashtirgan</i> so'z
>
> Pastki <sub>indeks</sub> va Ustki <sup>indeks</sup>

Majud urg'u beruvchilar:

| Teg                  | Tavsif                                    |
|----------------------|-------------------------------------------|
| `<b>...</b>`         | <b>Qalin matn</b>                         |
| `<i>...</i>`         | <i>Kursiv matn</i>                        |
| `<mark>...</mark>`   | <mark>Sariq fondagi matn</mark>           |
| `<small>...</small>` | <small>Kichchiklashtirilgan matn</small>  |
| `<del>...</del>`     | <del>O'chirilgan matn</del>               |
| `<ins>...</ins>`     | <ins>Osti chizilgan</ins>                 |
| `<sub>...</sub>`     | <sub>Pastki matn</sub>                    |
| `<sup>...</sup>`     | <sup>Ustki matn</sup>                     |

### 1. Qalin matnlar

Paragraf ichidagi bir ikkita so'zlarni yiriklashtirib ko'rsatish uchun, aslida 2 ta teg mavjud:

1. `<b>..</b>`
2. `<strong>..</strong>`

Ikkalasiyam so'zni qora va qalin shaklida ko'rsatadi, va bir biridan deyarli farqi yo'q. Kichkinagina farqi kontekstta `<b>` tegi faqat visual effect beradi va orasidagi so'z hech qanday ahamiyatga ega emas, ammo `<stong>` elementi katta ahamiyatga ega bo'lgan so'zlarni belgilaydi.

~~~html
<b>Qalin muhim emas so'z</b>
<strong>Qalin muhim so'z</strong>
~~~

### 2. Kursiv

Buning uchun ham 2tasi mavjud:

1. `<i>..</i>` - Atamalar, begona so'zlar, fikrlar va h.k kabi mahsus so'zrda qo'llaniladi
2. `<em>..</em>` - So'zlarga urg'u beradi, va unga e'tibor qaratishlikni chaqiradi

:::main{#success}
Vizual ravishda ular o'rtasida hech qanday farq yo'q!
:::

### 3. Orqa fon

HTML `<mark>` elementi belgilanishi yoki ajratilishi kerak bo'lgan matnni belgilaydi. 

Asosan biz kitob o'qiyotkanimizda kerakli qatorlarni sariq yoritgich markerini ishlatamiz, shu marker o'rninida HTML da `<mark>` tegi bor.

![MARKER](https://i.ibb.co/vZSS8GL/Group-5-1.png)

~~~html
<p>
    Бир куни падари бузрукворимиз — <mark>Амир Тарағой баҳодир</mark> кўп қўйларни менга бериб, 
    Самарқанд бозорига савдога йўлладилар.
<p>
~~~

### 4. Qo'shilgan va O'chirilgan so'zlar

HTML `<del>` elementi (tegi) hujjatdan o'chirilgan matnni belgilaydi. 

Brauzerlar, odatda, bu teg orasidagi matin *ustiga* <del>chiziq tortadi</del>.

Uning teskarisi bo'lgan teg bu `<ins>` tegi. Bu teg so'zni aynan qo'shilganini ifodalaydi.

Brauzerlarda, orasidagi matin *ostiga* <ins>chiziq tortadi</ins>.

~~~html
<h1>Mening sevgan futbolchim bu:
    <del>Messi</del> <ins>Eldor!</ins>
</h1>
~~~

### 5. Indeks

Matematika, Kimyo va Fizika formularini yozishda biz asosan *pastki* <sub>indekslardan</sub>, va bazida *ustki* <sup>indekslardan</sup> foydalanamiz.

#### Pastki indeks

Indeksni so'zning pastgi qismiga yozish uchun `<sub>...</sub>` teglari ishlatiladi:

~~~html
H<sub>2</sub>O - bu suv formulasi
~~~

#### Ustki indeks

Indeksni so'zning tepa qismiga yozish uchun `<sup></sup>` teglari ishlatiladi:

~~~html
2<sup>2</sup> + 2<sup>3</sup> = 12
~~~

#### 6. Kichik matinlar

HTML `<small>` tegi kichikroq matnni belgilaydi (mualliflik huquqi va boshqa sharhlar kabi).

~~~html
<p>Oddiy matin</p>
<p><small>Kichraytirilgan main</small></p>
~~~

## CSS ning o'rni

Aslida tepadgi teglar ko'proq sayt yasahda emas, balkim blog uchun *maqolalar* yozishda qo'llaniladi.

Sayt yasashda biz asosan o'sha-o'sha `p`, `span` (Xali bu tegni o'tmadik!) teglari va CSS orqali xohlagan uslublarni beramiz.

Masalan `mark` faqat sariq rangga bo'yasa biz CSS yordamida uning orqa fonini, va rangini o'zgartsak bo'ladi:

~~~html
<mark>
    Marker
</mark>

<style>
    mark {
        background-color: white;
        color: blue;
    }
</style>
~~~

Va InshaAllah *CSS* dan darsimizni, albatta HTML dan so'ng o'rganishni boshlaymiz.
