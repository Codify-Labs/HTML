Unchalik muhim bo'lmagan, lekin asqotishi mumkun bo'lgan teglar:


| Teg         | Ekranda ko'rsatadi:                  |
|-------------|--------------------------------------|
| `<code>`    | Dasturlash kodini                    |
| `<kbd>`     | Klaviatura belgilarini               |
| `<samp>`    | Kompyuter javoblarini                |
| `<pre>`     | Matnni abzaslar bilan                |
| `<bdo>`     | Matn yo'nalishini o'zgartirib        |
| `<address>` | Bog'lanish ma'lumotlarini belgilaydi |

#### 1. *code*

HTML kodi elementi *dasturlash tillari kodlarini* ko'rsatich uchun ishlatiladi. Ichidagi matn standart *monospace* shriftida ko'rsatiladi.

~~~html
<code>
  function start() {
    echo "Assalom!";
  }

  start();
</code>
~~~

:::main{#info}
`code` inline (cheklangan) element!
:::

#### 2. *pre*

`pre` matindagibarcha bo'shliqlarni va xat boshilarni saqlab qoladi:

~~~html
<pre>
  <code>
    function start() {
      echo "Assalom!";
    }

    start();
  </code>
</pre>
~~~

Matinlar bilan ham ishlatsa bo'ladi:

~~~html
<pre>
  Muhandis - qurilmaning ishlashini tushuntirib bera oladigan, 
  lekin nima uchun 
  
  ishlamayotganini tushuntirolmaydigan kishi.

  M.Tetcher
</pre>
~~~

#### 3. *bdo*

Teskari matin ekanligag ishora beradi:

:::main{#info}
Matinni o'girish uchun `dir="rtl"` attributidan foydalaning 
:::

~~~html
<bdo dir="rtl">Teskari yozilgan matin!</bdo>
~~~

Mana shuni ham sinab ko'ring:

~~~html
<p dir="rtl">Teskari yozilgan matin!</p>
~~~

:::main{#info}
`rtl` qiymati bu *arab* yozuvi ekanligiga ishora!

1. right-to-left (RTL), ya'ni o'ngdan chapga
2. left-to-right (LTR), ya'ni chapdan o'ngga
:::

Qolgan teglarni o'zingiz sinab ko'ring!
