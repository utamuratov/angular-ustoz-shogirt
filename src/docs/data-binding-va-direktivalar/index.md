---
keyword: DataBindingVaDirektivalarPage
---

Ushbu darsda siz Angular ilovasida data binding usullarini va direktivalar bilan ishlashni o'rganasiz. Shuningdek, Angular 17+ versiyasida kiritilgan yangi Control Flow sintaksisi bilan tanishasiz.

## Mundarija

1. **Data Binding turlari:**
   - Interpolation: `{{ '{{variable}}' }}`
   - Property Binding: `[property]="value"`
   - Event Binding: `(event)="handler()"`
   - Two-way Data Binding: `[(ngModel)]="variable"`
2. **Direktivalar:**

   ```html name="Structural directives"
   *ngIf, *ngFor, \*ngSwitch
   ```

   - Attribute directives: `ngClass`, `ngStyle`
   - Custom directives yaratish

3. **Control flow:** `@if` , `@for` , `@switch`

## 1. Data Binding nima?

**Data Binding** - bu component class (TypeScript) va template (HTML) o'rtasida ma'lumotlarni avtomatik sinxronlash mexanizmidir. Ya’ni sodda tilda aytganda componentdagi ma’lumotni templateda chiqarish, templatedan turib biror harakat haqida componentni xabardor qilish va shuningdek templatedan turib componentdagi o’sha ma’lumotga o’zgartirish kirita olish tushiniladi.

### 1.1 Interpolation (Interpolyatsiya)

Interpolation - bu componentdagi o'zgaruvchilarni HTML ga chiqarish usuli.
**Sintaksis:** `{{ variable }}`

**Misol:**

```tsx
// calculator.component.ts
export class CalculatorComponent {
  title = 'Matematika Kalkulyatori';
  result = 0;
  userName = 'Utamuratov';
}
```

```html
<!-- calculator.component.html -->
<h1>{{ '{{ title }}' }}</h1>
<p>{{ '{{ result }}' }}</p>
<p>{{ '{{ userName }}' }}</p>
```
