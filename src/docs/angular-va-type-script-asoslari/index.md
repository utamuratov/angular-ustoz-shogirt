---
keyword: AngularVaTypeScriptAsoslariPage
---

Ushbu dars Angular va TypeScriptga kirish darsi bo'lib unda Angular nima ekani, u uchun kerak bo'ladigan muhitni qanday sozlash, TypeScript asoslari haqida boshlang'ich ma'lumotlar beriladi.

## Mundarija

1. **Angular nima va nima uchun kerak?**
   - Single Page Application (SPA) tushunchasi
   - Angular vs oddiy JavaScript
   - Angular versiyalari. Zamonaviy Angular(14+) afzalliklari
2. **Muhitni sozlash:**
   - Node.js va npm o'rnatish
   - Angular CLI o'rnatish: `npm install -g @angular/cli`
   - Birinchi loyihani yaratish: `ng new math-platform`
3. **TypeScript asoslari:**
   - O'zgaruvchilar: let, const
   - Turlar: string, number, boolean, any
   - Interface va type
   - Funksiyalar va arrow functions
4. **Loyiha strukturasi:**
   - src/app papkasi
   - Component tuzilishi
   - Module nima?

## Angular nima va nima uchun kerak?

**Angular** — bu Google tomonidan ishlab chiqilgan **frontend framework** bo’lib web saytlar, web ilovalar, katta va murakkab interfeyslar yaratish uchun ishlatiladi.

Angular yordamida:

- Kod tartibli bo‘ladi
- Katta loyihalarni boshqarish osonlashadi
- Xatolar kamayadi
- Tezkor va interaktiv ilovalar yaratiladi

<aside>

> **Note**
> Oddiy qilib aytganda: Angular — bu HTML + CSS + JavaScript asosida websaytlarni oson, tez va professional darajada qura olish imkoniyatini beruvchi framework(yozilgan qonun qoida, konsepsiya va kutubxonalar to’plami)

</aside>

<iframe 
  width="560px"
  height="315px" src="https://www.youtube.com/embed/trH-ePyM5uI" title="#0 Kurs kimlar uchun?  Angular nima? | Angularga samarali kirish | 100 daqiqada" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe 
  width="560px"
  height="315px" src="https://www.youtube.com/embed/pI-9RB78yaw" title="#1 Nima uchun Angular | Angularga samarali kirish | 100 daqiqada" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Single Page Application (SPA) nima?

### Oddiy sayt qanday ishlaydi?

Oddiy saytlar har sahifa almashganda Serverga qayta so‘rov yuboradi va sahifa to‘liq yangilanadi. Bu esa sayt sekin yuklanishi, ortiqcha internet sarf bo’lishiga sababchi bo’ladi.

### SPA qanday ishlaydi?

Faqatgina **bitta HTML sahifa** yuklanadi va qolgan sahifalar, o’zgarishlar JavaScript orqali sahifa yangilanmasdan to’ldirib, o’zgarib boraveradi. Bu esa sayt samaradorligini yanada oshirib beradi ya’ni dasturlash tilida aytganda “performance’i yuqori” bo’ladi.

### SPA afzalliklari:

- Juda tez ishlaydi;
- Foydalanuvchi uchun qulay interfeys taqdim qiladi (yuqori UX);
- Mobil ilovaga o‘xshab ishlaydi;

“SPA ni Angularga qanday aloqasi bor o’zi?” degan savol sizda tug’ilgan bo’lsa javobi oddiy. Angular - Single Page Application yaratish uchun **eng kuchli frameworklardan biri**.

## Angular vs oddiy JavaScript

| Oddiy JavaScript       | Angular               |
| ---------------------- | --------------------- |
| Kichik loyihalar uchun | Katta loyihalar uchun |
| Strukturasi yo‘q       | Qattiq struktura      |
| Hammasi qo‘lda         | Ko‘p narsa avtomatik  |
| Kod chalkashib ketadi  | Kod tartibli          |

<aside>
💡

**Xulosa**

Agar katta va kengayib boradigan loyiha qilmoqchi bo‘lsangiz — Angular to’g’ri tanlov.

</aside>

**⁉️ Topshiriq 1**
Siz HTML orqali oddiy input va uning yonida ikkita `+` `-` tugmalarini yasashingiz kerak. `+` tugmasi bosilganda input ichidagi qiymat 1 ga oshishi, `-` tugmasi bosilganda esa 1 ga kamayishi kerak. Bu funksional JavaScript orqali qilinishi kerak.
Xo’sh, bu topshiriqni qanday qilasiz? Amalda qilib ko’ring yoki topshiriq juda oddiy bo’lsa qanday qilishingizni miyangizda o’ylab, o’zingizni interviewdaman deb tasavvur qilib unga to’liq javob berishga harakat qiling.

![increase-decrease](/docs/increase-decrease.png)

## Angular versiyalari. Zamonaviy Angular(14+) afzalliklari

Angular:

- Har 6 oyda yangilanadi
- Eski versiyalar sekin-asta qo‘llab-quvvatlanmaydi

### Angular 14+ afzalliklari:

- Tezroq ishlaydi
- Standalone Components (Module’siz ishlash)
- Kamroq kod
- Zamonaviy yondashuv

<aside>
💡

Ushbu kursda **zamonaviy Angular (14+)** ishlatiladi.

</aside>

## Muhitni sozlash (Environment Setup)

Angular bilan ishlash uchun quyidagilar kerak:

### 1. Node.js va npm

- Node.js — JavaScript’ni serverda ishlatadi
- npm — paket menejeri

🔗 Yuklab olish: [https://nodejs.org](https://nodejs.org/) (LTS versiyasini tanlang)

Tekshirish:

```bash
node -v
npm -v
```

### 2. Angular CLI o‘rnatish

Angular CLI — Angular loyihalarni boshqarish uchun yordamchi ish quroli.

```bash
npm install -g @angular/cli
```

Tekshirish:

```bash
ng version
```

### 3. Birinchi loyihani yaratish

```bash
ng new math-platform
```

Savollarga tavsiya:

- Standalone: **Yes**
- Routing: **Yes**
- Style: **CSS**

Loyihani ishga tushirish:

```bash
cd math-platform
ng serve
```

Brauzerda:

```
http://localhost:4200
```

🎉 Sizning birinchi Angular ilovangiz ishga tushdi!

<iframe 
  width="560px"
  height="315px" src="https://www.youtube.com/embed/ZIvAmuck4QA" title="#2 Angular muhitini sozlash | Angularga samarali kirish | 100 daqiqada" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## TypeScript asoslari

Angular **TypeScript** bilan yoziladi. TypeScript — bu JavaScript’ning kuchliroq versiyasi.

### O‘zgaruvchilar

```ts
let age: number = 15;
const name: string = 'Ali';
```

- `let` — o‘zgaruvchan
- `const` — o‘zgarmas

### Asosiy turlar (Types)

```ts
let isActive: boolean = true;
let score: number = 100;
let title: string = 'Matematika';
let data: any = 'istalgan narsa';
```

📌 `any` — imkon qadar kam ishlatiladi.

### Interface va type

**Interface** — obyekt tuzilmasini belgilaydi.

```ts
interface Student {
  id: number;
  name: string;
  grade: number;
}
```

**Type** ham shunga o‘xshash:

```ts
type Course = {
  id: number;
  title: string;
};
```

### Funksiyalar

```ts
function add(a: number, b: number): number {
  return a + b;
}
```

### Arrow function

```ts
const multiply = (a: number, b: number): number => a * b;
```

<iframe 
  width="560px"
  height="315px" src="https://www.youtube.com/embed/w7fLeB2edpY" title="2-dars. TypeScript. Everyday types | BeMiddle" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Angular loyiha strukturasi

`src/app` papkasi loyihaning asosiy papkasi

```
src/
 └── app/
     ├── app.component.ts
     ├── app.component.html
     ├── app.component.css
```

### Component nima?

Component — bu:

- HTML (ko‘rinish)
- CSS (dizayn)
- TypeScript (mantiq ya’ni logika)

bir joyda saqlanadigan qism.

```ts
@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
})
export class AppComponent {}
```

### Module nima? (Qisqacha)

Module:

- Ilovani bo‘limlarga ajratadi
- Component, service’larni birlashtiradi

<aside>
💡

Hozirgi zamonaviy Angulardagi **Standalone Component** sababli module deyarli ishlatilmaydi.

</aside>

[#5 Angular Legolari: Component, Template, Logika va Service | Angularga samarali kirish | 100 daqiqa](https://youtu.be/AcNUd3C7KMc)

[#6 Angular loyiha strukturasi | Boshlang'ich bilimlar | Angularga samarali kirish | 100 soniyada](https://youtu.be/2DzboodOY38)

## Savollarga javob bering!

1. Angular nima va nima uchun kerak?
2. SPA nima?
3. Angular CLI nima vazifa bajaradi?
4. TypeScript nima uchun kerak?
5. Component deganda nimani tushunasiz?

## Test

1. Angular loyihasini yaratish uchun qaysi buyruq ishlatiladi?\
   A) `npm create angular`\
   B) `ng new project-name`\
   C) `angular init`\
   D) `npm install angular`
2. Component yaratish buyrug'i:\
   A) `ng create component`\
   B) `ng add component`\
   C) `ng generate component`\
   D) `ng new component`
3. TypeScript faylining kengaytmasi:\
   A) .js\
   B) .ts\
   C) .jsx\
   D) .angular
4. Angular loyihasini ishga tushirish:
   A) `npm start`\
   B) `ng serve`\
   C) `node app.js`\
   D) `angular run`
5. Component decoratori qaysi faylda yoziladi?\
   A) `.html`\
   B) `.css`\
   C) `.ts`\
   D) `.json`

[Quiz Bot](https://t.me/QuizBot?start=70iD5PoX)

## Amaliy vazifa

1. Angular loyihaningiz ichida `math-operations` nomli yangi komponent yarating
2. Komponentda ikkita input maydoni (son1, son2) va 4 ta tugma (+, -, \*, /) yarating
3. Root component ya’ni app.component.ts (yoki app.ts) da esa ushbu componentni chaqirib ishlating.

![calculator](/docs/calculator.png)
