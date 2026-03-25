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
