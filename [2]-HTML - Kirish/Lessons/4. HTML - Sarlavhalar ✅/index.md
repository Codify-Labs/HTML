> <h1>Sarlavha - 1</h1>
> <h2>Sarlavha - 2</h2>
> <h3>Sarlavha - 3</h3>
> <h4>Sarlavha - 4</h4>
> <h5>Sarlavha - 5</h5>
> <h6>Sarlavha - 6</h6>

## Sarlavha Yaratish

HTML da 6 "qatlam" sarlavha mavjud.

`<h1>...</h1>` - Asosiy, eng katta sarlavha

`<h2>...</h2>` - Ikkinchi qatlam sarlavha. `h1` dan sal kichikroq.

`h2` danda kichikroq sarlavha yaratish kerak bo'lsa `h3` va to `h6` larni ishlatsa bo'ladi.

Sinab ko'ring:

~~~html
<h1>Sarlavha 1</h1>
<h2>Sarlavha 2</h2>
<h3>Sarlavha 3</h3>
<h4>Sarlavha 4</h4>
<h5>Sarlavha 5</h5>
<h6>Sarlavha 6</h6>
~~~

Aslida *CSS* yordamida xohlagan matinni saralavhaga aylantirish, uning rangini o'zgartish va ustida turli xil amallarni bajarsak bo'ladi:

~~~html
<h4>CSS yordamida kattalashtirilgan Sarlavha - 4</h4>

<style>
    h4 {
        font-size: 3rem;
    }
</style>
~~~

### Qisqa *CSS* tushunturilish

*CSS* yordamida matinni va xohlagan HTML tegga ishlov berishimiz mumkun ekan.

:::main{#info}
#### Eslab qoling!

CSS kod har-doim HTML da `<style>...</style>` teglari orasida yoziladi.
:::

CSS bo'yicha ham darsligimiz [mavjud](), lekin uni o'rganishni faqatgina HTML kursidan so'ng boshlashni maslaxat beraman.

---

Shunday bo'lsada CSS xaqida ozgina-ozgina tushunchalar olish, kelajakda CSS kursini o'rganayotkan o'quvchiga, ya'ni sizga, yengillik tug'diradi.

Demak, shu CSS kodimizning mazmuni quyidagicha:

~~~html
<h4>CSS yordamida kattalashtirilgan Sarlavha - 4</h4>

<style>
    h4 {
        font-size: 3rem;
    }
</style>
~~~

1. Biz `h4` Sarlavhasini yaratdik
2. CSS kod yozish uchun `style` teginin ochib oldik
3. `style` teglari orasiga biz shu kodni joyladik:

~~~css
h4 {
    font-size: 3rem;
}
~~~

Mazmuni `h4` elementi tanlab uning xajmini `3rem`ga (bu HTML-ning o'lchov birligi, CSS darsligimizda uni chuqurroq ko'rib chiqamiz) o'zgartir.

CSS da HTML *tegni* tanlash uchun `teg nomi` + `{` + `}` va uning orasidan, tanlangan tegga ishlov beramiz, bizda esa `font-size`, ya'ni tarjimada *shrift o'lchami*ni `3rem`ga o'zgartir.

Qo'shimcha, rangini o'zgartirmoqchi bo'lsangiz `color` + `RANG NOMI` qo'llaniladi:

:::main{#success}
Bu yerda *RANG NOMI* o'rniga ingliz tilidagi rang nomlari qo'yiladi, bizda *blue* rangi, ya'ni *ko'k*
:::

~~~css
h4 {
    font-size: 3rem;
}

h4 {
    color: blue;
}
~~~

Bu uzun kodni qisqaroq qilsakda bo'ladi:

~~~css
h4 {
    font-size: 3rem;
    color: blue;
}
~~~

:::main{#warn}
`h1`, `h2` teglari sahifadagi muhim narsalarni belgilashda ishlatilinadi

`h1` ning o'rniga, stil berish orqali `h4` ishlatish maslahat etilmaydi, sababi ular qidiruv tizimlariga (GOOGLE, YANDEX) sahifadagi muhim jihatlarni aniqlashda va indekslashda yordam beradi.

Shundan kelib chiqib, *sarlavhalar* sahifaning mazmuniga mos keladigan tartibda ishlatilishi kerak
:::
