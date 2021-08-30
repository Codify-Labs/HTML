## Attributlar nima?

Attributlar, teglar bilan ishlashda eng kerakli narsa (o'zbekcha: "Xususiyat" ma'nosi).

Attributlar teglarda qo'shimcha funksional yaratishga va ularga xususiyat berishga imkon beradi. Attributlarni [self-closing](#self_closing)lardan boshqa, xohlagan teglarga qo'shsa bo'ladi.
  
Keling atributlarning qanday ajoyibot ekanligini, va ularni foydalanishning ba'zi misollarini ko'rib chiqaylik.

## Attributlarning sintaksisi

Attributlarni ishlatishdagi bazi bir qoidalar:

1. Deyarli hamma teglarda attribut qo'shish imkoni bor
2. Attributlar teglarga turli xil funksional qo'shadi
3. Ular *ochilish* tegi ichidan yoziladi
4. Sintaksisi *nom="qiymat"* shaklida bo'ladi.

![ATTRIBUTE](https://imglink.io/ib/78CLrKgmGc.png)

Attributga misol:

~~~html
<p title="Soat 21:00 - da">
    Barcelon vs Real Madrid
</p>
~~~

:::main{#info}
O'ng tarfdagi *redaktorimizda* sinab ko'ring!
:::

Sichqonchani *Barcelon vs Real Madrid* matini ustiga oborib 1 soniya ushlab tursak, *Soat 21:00 - da*  sharhi chiqadi.

Mana shunday ko'plab funksinallar aynan *attributlar* yordamida bajariladi. Masalan `onclick="alert('Mening ismim ...')"` attributi, teg ustiga bosilganda 👆 *Mening ismim ...* xabarini ekranga chiqaradi.

Mavjud bo'lgan *attributlar* yetarlicha (100talab mavjud):

`href`, `title`, `lang`, `class`, `id`, `onclick` va h.k. Lekin, eng kerakli (90% vaziyatlarda ishlatiladigan) attributlarning xammasini ko'rib o'tamiz.

Keyingi qadam bizga kerakli bo'lgan barcha *attributlarning* hammasini, qayerda? qanday? va nima uchun? degan sorovlar orqali birin ketin ko'rib chiqish.

### 1. *title* attributi

##### Nima uchun?

*Title* - attributi HTML elementning (HTML teg) mazmuni haqida tushuntirish matnini taqdim etish uchun ishlatiladi.

##### Qayerda?

:::main{#success}
#### Eslab qoling

Hamma attributlar Tegning ochilish qismida yoziladi. Tepada ko'rsatilgan rasmga qarang!
:::

Shuning uchun <strong>qayerda?</strong> so'rovini olib tashlaymiz.

##### Qanday?

Xuddi `attributNomi="Qiymat"` shaklida. Bu yerda `title="qiymat"` shaklida bo'ladi.
  
Bu qanday ishlashini tushunish uchun quyidagi misolni sinab ko'ring.
  
~~~html
<h1 title="Davlat Test Markazi">
    DTM
</h1>
~~~

Sichqonchani *DTM* qisqartmasi usitga oborganimizda, *Davlat Test Markazi* izohini taqdim etadi.

### 2. *style* attributi

##### Nima uchun?

`<style>...</style>` teglari o'rnini bosish uchun. Style atributi to'g'ridan-to'g'ri element ichida rang, shrift, va boshqalar kabi CSS uslublarini va oidalarini belgilashda imkon beradi.

Keling, qanday ishlashini ko'rib, amalda sinab ko'raylik:
  
~~~html
<p style="color: blue;">
    Ko'k matin
</p>
~~~

Mana shuning bilan bir natija, farqi *style="color: blue;"*  attributi bilan kodimiz ancha qisqaroq:

~~~html
<p>
    Ko'k matin
</p>

<style>
    p {
        color: blue;
    }
</style>
~~~

### 3. *src* attributi

##### Nima uchun?

Ekrang rasm chiqarish uchun qo'llaniladi. Va `<img />` tegi bilan shartli tarzda ishlatiladi.

:::main{#info}
### Yangi teg

Ekranga rasm `<img />` tegi + `src` atributi orqali uzatiladi
:::

##### Qanday?
  
`<img src="rasm-linki"/>` - bu yerda *src* qiymatiga rasm linkini joylaymiz.

O'zbekiston flagining [rasmi](https://cdn.britannica.com/47/7247-004-44F420D7/Flag-Uzbekistan.jpg) (https://cdn.britannica.com/47/7247-004-44F420D7/Flag-Uzbekistan.jpg)

~~~html
<img src="https://cdn.britannica.com/47/7247-004-44F420D7/Flag-Uzbekistan.jpg" />
~~~
  
Bu yerda *src* attributimizning *qiyamtiga* xohlagan rasm linkini joylasak bo'ladi.

Shularni sinab ko'ring (Rasm *linkini* nusxalab *src* ga qo'yasiz):
  
1. [Messi](https://imgresizer.eurosport.com/unsafe/1200x0/filters:format(jpeg):focal(1404x222:1406x220)/origin-imgresizer.eurosport.com/2021/05/17/3134648-64248688-2560-1440.jpg)
2. [Kuz](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS1D07TzQkGLrMWn9je6vF_3udKttdnB9tCI3s2cenBiyRHS_bgtV0uMDq_Ff3oGhXVnFY&usqp=CAU)
3. [Palma](https://www.industrialempathy.com/img/remote/ZiClJf-1920w.jpg)
  
### 4. *Class* va *id* attributlari
  
Bular siz uchun ajoyib kashfiyot bo'ladi! Ishonavering.

Bular orqali siz CSS da mojizalar qilishni boshlaysiz. Lekin xozircha bu attributlarni o'rganish sal ertaroq, shuning uchun keyinroqqa qoldiramiz.

Attributlar anchadan-ancha ko'p, shuning uchun bularning ko'pini amalda <strong>yangi teglar</strong> bilan o'rganayotkanimizda, ularga attributlar orqali yangi-yangi funcksionallar qo'shib, amalda sinab, qo'llab ko'pini InshaAllah o'rganasiz!
