# One way binding

## String interpolation vs Property binding:

- `Class component` to `Template view`
- Syntax `string interpolation`: `{{expression}}`
- Syntax `property binding`: `[property] = "expression"` or `bind-property = "expression"`
- `Disabled`, `Hidden`, `Checked` not work in String interpolation

- `Attribute` vs `Property`:
  - `Attribute`: Represents the initial value and does not change(`aria-label`, `aria-hidden`, `aria-expanded`, `aria-control`, `data-id`, `data-name`, `data-value`, `colspan`). Syntax: `[attr.attribute] = "expression"`
  - `Property`: Represents the current value and can change.

## Event binding:

- `Template view` to `Class component`
- Syntax: `(event)=yourFunction($event)`.

# Two way binding:

- Combine: Property binding + Event binding
- Note: Install `ngModel` and `imports` to AppModule
- Syntax: `[(ngModel)]="propertyChange"`
