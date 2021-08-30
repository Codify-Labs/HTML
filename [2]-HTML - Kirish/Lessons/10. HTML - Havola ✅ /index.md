Havola bu foydalanuvchilarga bir sayttan ikkinchi saytga o'tishni ta'minlaydi.

Sichqonchani havola ustida obirganda, sichqoncha kichik qo'lga aylanadi 👆.

Misol tariqasida [google.com](#) sayti:

![LINK](https://i.ibb.co/NCwB26G/LINK.gif)

### Havola sintaksisi

Havolalar `<a>` HTML elementi (tegi) yordamida yaratiladi. Orasiga beriladikan matin, bosish mumkun bo'lgan havolaga aylanadi, va `href` attributi yordamida saytga havola qoldirasiz:

:::main{#info}
Havola `inline` (Cheklangan) element
:::

~~~html
Mana shu <a href="https://kun.uz">havola:</a>
~~~

Qiziqarli tomoni `a` tegi kontentiga nima joylasangiz o'sha havolaga aylanadi.

Misol rasm joylaymiz:

~~~html
Rasm bilan havola
<a href="https://kun.uz">
    <img
        src="https://i.ibb.co/Yj4M1f2/1200px-Facebook-Logo-2019.webp"
        width="100"
        height="100"
    />
</a>
~~~

:::main{#success}
Rasmgning o'chamlarini `width` va `height` orqali o'zgartsa bo'ladi.
:::

Havolaning umumiy tuzilishi:

![LINK_TAG](https://i.ibb.co/QKb36dt/Group-12-1.png)

### Havola ko'rinishi

Shuningdek, havolalar barcha brauzerlarda quyidagicha ko'rinish oladi:

- Xali ustiga bosilmagan havola chizilgan va ko'k rangda
- Bosilgan havola chizilgan va binafsha rangda
- Faol havola (Ustiga bosip turulganda) chizilgan va qizil rangda

:::main{#info}
Albatta *CSS* yordamida buni o'zgartirsa bo'ladi.
:::

### *Target* Attributi

Odatta, `a` tegini bosganingizda shu saytning ustidan yangi saytga o'tiladi.

`Target` attributi havolani qayerdan ochilishini belgilaydi.

Uning qiymatiga 4ta qiymat turini berish mumkun, ular quyidagilar:

#### 1. `_self`

Hujjat bosilgan oynadan ochadi. Yozish shart emas! (*default* qiymat)

#### 2. `_blank`

Saytni yangi *tabdan* (oynadan) ochadi.

#### 3. `_parent`

Saytni yuqori freymda ochadi

#### 4. `_top`

Saytni oynaning to'liq qismida ochadi

Eng ko'p qo'llaniladigani bu `_blank` qiymati:

~~~html
<a target="_blank" href="https://google.com">Google.com</a>
~~~

### Absolut URL vs Relative URL

Tepadagi barcha misollarda *src* attributi qiymatiga *absolut* sayt manzili kiritildi.

:::main{#success}
Sayt manzilini *URL* deb nomlash tog'riroq bo'ladi
:::

![IMAGE_URL](https://i.ibb.co/tsB9k5J/Group-14.png)

`https://devilla.uz/about`ning Relative va Absolut URL lari:

1. Relative URL sayt manzilining (URL) ning *directory* (*/about*) qismi.
2. Absolut URL bu sayt manzilining (URL) to'liq nomi: `https://devilla.uz/about`.

Agarda sizning saytingiz [devilla.uz](#) *domenida* bo'lsa va shu saytning o'ziga `https://devilla.uz/about` havolasi bilan yo'naltirmoqchi bo'lsangiz *directory* qismini yozish kifoya:

~~~html
<a href="/about">devilla.uz<a>
~~~

Mana shu ham bir hil natijani beradi:

~~~html
<a href="https://devilla.uz/about">devilla.uz<a>
~~~

Lekin siz [devilaa.uz](#)dan turib [google.com](#) saytiga yo'naltirmoqchi bo'lsangiz, Absolut URL ishlatishingiz shartli bo'ladi:

~~~html
<a href="https://google.com">google.com<a>
~~~
