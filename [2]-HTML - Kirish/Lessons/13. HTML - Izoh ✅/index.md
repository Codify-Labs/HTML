Izoh - bu yozilayotkan kodning tarkibiy qismi bo'lip, dasturlash tili yoki brazuerda e'tiborga olinmaydi. 

Kodga komment yozish shunday amaliyotki, hujjatni yoki yozilgan parcha kodlarni tasvrilab berish, eslatmalar qoldirish va tushuntirishdir.

Izohlar sizdan boshqa odam, siz yozgan kodni nima? va nima uchun? ekanligini tushinishda qo'l keladi.

#### 1. Izoh sinktaksisi

Izohlar HTML da `<!--` (ochish qismi) va `-->` (yopish qismi) orasida yoziladi.

E'tibor bering, izohni ochish qismida undov belgisi (!) bor.

~~~html
<!-- Men Izohman -->

<!-- Men
    yangi 
    xat boshi bilan ham, yoki qisqa 
    bir qatordan ham yozilishim mumkun.
-->

~~~

Ularni qisqa bir qatordan, yoki bir nechta qatordan yozishingiz mumkun.

~~~html
<!-- Bugungi kun yangiliklari kodi -->
<h1>Bugungu kun yangiliklari:</h1> 

<!-- Birinchi yangilik -->
<h4>1. Bugun qashda yangi robot ishlab chiqildi!</h4>
<p>Lorem ipusm ...</p>

<!-- Ikkinchi yangilik -->
<h4>2. O'zbekistonda yangi codify.uz platformasi ishga tushdi!</h4>
<p>Lorem ipusm ...</p>

<!-- Uchunchi yangilik -->
<h4>3. Yangi O'zbekiton!</h4>
<p>Lorem ipusm ...</p>
~~~

HTML izohlarni ekranga chiqarmaydi, lekin izohlar manba kodida saqlanib qoladi.

:::main{#info}
Kodni redaktorda sinab ko'ring.
:::

HTML kodlarni ham izoh orasiga qo'shsak bo'ladi, va u ekranga chiqarilmaydi:

~~~html
<!--
    Chrome brauzeri logosi va u ekranga chiqmaydi
    <img 
        src="https://html.com/wp-content/plugins/htmlcodetutorial-plugin/assets/images/chrome-true.png"
    />
-->

<p>Lorem ipsum dolor..</p>
~~~

### Izoh tartiblari

Izoh yozsihda xech qanday shart yo'q, muhimi o'zingiz uchun qulay bo'lishi, va tartibsizlikni tog'irlashi (uni keltirib chiqarishi emas).

Namuna sifatida [instrument.uz](https://instrument.uz) sayti. U yerda izohlar matin bilan emas, aksincha `<!-- ========== -->` shaklida yozilgan:

~~~html

<h1>Bugungu kun yangiliklari:</h1> 

<!-- =============== -->
<h4>1. Bugun qashda yangi robot ishlab chiqildi!</h4>
<p>Lorem ipusm ...</p>

<!-- =============== -->
<h4>2. O'zbekistonda yangi codify.uz platformasi ishga tushdi!</h4>
<p>Lorem ipusm ...</p>

<!-- =============== -->
<h4>3. Yangi O'zbekiton!</h4>
<p>Lorem ipusm ...</p>
~~~
