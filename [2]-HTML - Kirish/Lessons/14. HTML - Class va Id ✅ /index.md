Teglarga CSS bilan *uslub* berishni yuzaki ko'rib o'tkandik.

~~~html
<h1>Alhamdulillah</h1>

<style>
    h1 {
        color: blue;
    }
</style>
~~~

Tepadagi HTML kodni chapda sinab natijasini ko'ring. Sarlavhamiz *ko'k* rangga bo'yaldi.

`h1` tegi ostidan yana bitta `h1` yaratib o'zingizning ismingizni yozing:

~~~html
<h1>Alhamdulillah</h1>

<h1>Babur</h1>

<style>
    h1 {
        color: blue;
    }
</style>
~~~

Ikkala sarlavha ham ko'k rangda. Xo'sh faqatgina birinchi sarlavhani ko'k rangga bo'yash uchun nima qilishimiz kerak? Saytta siz bir-hil teglardan yuzlab foydalanasiz, lekin bitta tegni uslubini o'zgartish, to'laligicha hamma mavjud teglar shu uslubga o'zgarishiga olib keladi.

Aynan shularni echish maqsadida *id* va *class* attributlari mavjud. Ular CSS va HTML da birlashtirishda asosiy bo'g'im!

Ular HTML tegni boshqa bir-hil teglardan ajratish uchun nomdir. Shu nom bilan CSS da kerakli tegni aniqlab unga uslublarni beramiz.

### 1. *id*

~~~html
<p>Babur</p>
<p>Jasur</p>
<p>Alisher</p>
<p>Ulug'bek</p>
<p>Qudrat</p>
~~~

Birinchi `Babur` paragrafini qizil rangga bo'yash kerak bo'lsa unga *id="qiymat"* beramiz. (*qiymat o'rnida qandaydir nom)

Masalan *qizil_rang* qiymatini beramiz:

~~~html
<p id="qizil_rang">Babur</p>
<p>Jasur</p>
<p>Alisher</p>
<p>Ulug'bek</p>
<p>Qudrat</p>
~~~

CSSda, HTML tegni *id* orqali nishonga olish uchun `#` + `id_nomi` shaklida yoziladi:

~~~css
#qizil_rang {
    ...
}
~~~

![ID](https://i.ibb.co/vx0BzWj/Group-19.png)

Shuni sinab ko'ring:

~~~html
<p id="qizil_rang">Babur</p>
<p>Jasur</p>
<p>Alisher</p>
<p>Ulug'bek</p>
<p>Qudrat</p>

<style>
    #qizil_rang {
        color: red;
    } 
</style>
~~~

Bitta hujjatning ikkita elementi *bir xil* identifikator bilan nomlanishi mumkin emas va har bir element *faqat bitta* identifikatorga ega bo'lishi mumkin.

:::main{#warn}
*ID* qiymati HTML hujjati ichida *yagona* va boshqa teglarda *qaytalanmasligi* kerak.
:::

Bu xato:

~~~html

<!-- ID qaytalanmasligi kerak! ❌ -->
<p id="qizil_rang">Babur</p>
<p id="qizil_rang">Ulug'bek</p>

<!-- Id faqat 1 qiymat olishi kerak! ❌ -->
<p id="bir ikki">Jasur</p>



<style>
    #qizil_rang {
        color: red;
    } 
</style>
~~~

## 2. *Class*

*Id* CSS bilan ishlashda ishimizni ancha osonlashtirdi, ammo o'z cheklovlari bilan ham ishimizni qiyinlashtirdi. Bitta uslubni qayta ishlatish uchun yangi *id* yaratishga to'g'ri keladi.

Echim esa oddiy *class* attributini ishlatish!

*id* dan farqi, CSS da *class* ni nishonga olish uchun `#` emas `.` - nuqta ishlatiladi:

~~~css
.qizil_rang {
    ...
} 
~~~

![CLASS](https://i.ibb.co/HrGsN3G/Group-20.png)

HTML teglarda esa:

~~~html
<p class="qizil_rang">Babur</p>

<style>
.qizil_rang {
    color: red;
} 
</style>
~~~

Xatto bir nechta qiymatlar joylash, va bitta *qiymatni* bir necha marotaba ishlatish mumkun:

~~~html
<p class="qizil_rang">Babur</p>

<h1 class="qizil_rang sarlavha_tegi | bir_nechta_klass">Sarlavha</h1>

<style>
.qizil_rang {
    color: red;
} 
</style>
~~~

*Class* mana shunday ajoyib qulayliklar keltirib chiqarishu orqali, barcha *CSS* freymvorklar undan foydalanishadi.

Bootstrap, TailwindCSS hammasi ishingizni *class*lar orqali CSS bilan bilan ishlashda osonlashtoradi va albatta kelajakda bu texnologiyalarni ham o'rganamiz.
