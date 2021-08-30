HTML da `<` yoki `>` belgilarini ishlatish xatoliklarga olib kelish ehtimoli katta. Sababi bular zaxiralangan belgilardir.

Klaviaturangizdan `©`, `®`, `€`, `→`, yoki `∑` belgilarini topa olmaysiz, ular cheklangan (Bunday belgilardan minglab mavjud, va klaviaturada hammasini chiqarish ilojsiz).

Shularning echimi HTML da aynan *belgilar*.

## Belgi sintaksisi

Belgi yaratish uchun 2ta sintksis mavjud:

1. Nom: `&belgiNomi;` - `&` + `belgi nomi` + `;`
2. Son: `&#belgiSoni;` - `&` + `#` + `belgi soni` + `;`

Masalan <strong>®</strong> (mualliflik huquqi) belgisini yozish uchun:

1. Nom bilan: `&reg;`  = ®
2. Son bilan: `&#174;` = ®

Ba'zi belgilar va ularning kodirovkasi (1. Nomi orqali, 2. Son orqali):

| Belgi | 1. Nom   | 2. Son    |
|-------|----------|-----------|
| <     | `&lt;`   | `&#60;`   |
| >     | `&gt;`   | `&gt;`    |
| ®     | `&reg;`  | `&#174;`  |
| ©     | `&copy;` | `&#169;`  |
| ∑     | `&sum;`  | `&#8721;` |
| →     | `&rarr;` | `&#8594;` |

To'liq ro'yhat bilan [shu yerda tanishing](https://unicode-table.com/ru/html-entities/).
