# One way binding

## 1. String interpolation vs Property binding:

- `Class component` to `Template view`
- Syntax `string interpolation`: `{{expression}}`
- Syntax `property binding`: `[property] = "expression"` or `bind-property = "expression"`
- `Disabled`, `Hidden`, `Checked` not work in String interpolation

- `Attribute` vs `Property`:
  - `Attribute`: Represents the initial value and does not change(`aria-label`, `aria-hidden`, `aria-expanded`, `aria-control`, `data-id`, `data-name`, `data-value`, `colspan`). Syntax: `[attr.attribute] = "expression"`
  - `Property`: Represents the current value and can change.

## 2. Event binding:

- `Template view` to `Class component`
- Syntax: `(event)=yourFunction($event)`.

# Two way binding:

- Combine: Property binding + Event binding
- Note: Install `ngModel` and `imports` to AppModule
- Syntax: `[(ngModel)]="propertyChange"`

# Directive

- Có `3` loại directives:
  - `Component directives`: có view template riêng, có style sheet riêng. Tạo ra các UI phức tạp và độc lập.
  - `Structure directives`: thay đổi cấu trúc DOM(thêm xóa phần tử). Syntax: `*ngDirective="expression | statement"`. Built-in: `*ngIf`, `*ngFor`, `*ngSwitch`
  - `Attribute directives`: được áp dụng như các attributes của phần tử. Do vậy không làm thay đổi cấu trúc DOM. Syntax: `[ngDirective]="expression"`. Built-in" `[ngClass]`, `[ngStyle]`, `[(ngModel)]`
